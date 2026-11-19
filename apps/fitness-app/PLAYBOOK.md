# Fitness app playbook: Google Stitch → Claude Code

Status: **idea / saved for later**. Owner wants to build their own fitness app
for their coaching business eventually.

Source of the idea: YouTube Short "Build apps with Claude Code plus Google
Stitch" (youtube.com/shorts/fwhcOK_OsRU). The video itself couldn't be watched
when this was saved; this playbook describes the general workflow the title
refers to. Update it if the owner shares the video's exact steps.

## The workflow in one line

Design the screens visually in **Google Stitch** (Google Labs: text or image
prompt → app screen designs, exportable as HTML/CSS or to Figma), then hand
the exported screens to **Claude Code**, which builds the real, working app
around them.

## Phase 0: Decide what the app is (do this in claude.ai, no code)

Answer these before designing anything:

1. **Who is it for?** e.g. the owner's 1:1 clients, group programme members,
   or the public.
2. **The one job it must do on day one** (the MVP). Typical coaching-app
   candidates:
   - Today's workout (exercises, sets/reps, video demo, rest timer)
   - Log weights/reps and see progress
   - Programme calendar (weeks/phases)
   - Check-ins (bodyweight, photos, sleep/energy, notes) and coach feedback
   - Habit tracker (steps, water, protein)
   - Messaging with the coach
   - Payments / subscription
3. **Pick 1–3 for version 1.** Everything else goes on a "later" list.
4. **Platform:** start as a **web app (PWA)** that installs on the phone home
   screen. It's the fastest and cheapest, with no App Store review. Move to a
   native app (Expo / React Native) later if needed.

## Phase 1: Design screens in Google Stitch

- Go to stitch.withgoogle.com (Google account needed), choose **Mobile**.
- One prompt per screen. Include the style so it matches the brand. Use a
  style file from `design/styles/` (e.g. Origin for calm/nature, Firm
  Foundations for cream/navy/serif).
- Prompt template:

  > Mobile app screen for a personal-training app. Screen: [Today's workout].
  > Shows: [workout name, 5 exercises with sets × reps, demo thumbnail,
  > "Start workout" button, rest timer]. Style: [paste the Essentials bullets
  > from the chosen design/styles file: colours with hex, fonts, corner radius,
  > button style]. Clean, lots of space, one primary action.

- Make 4–6 core screens: Home/Today, Workout in progress, Log set, Progress
  charts, Check-in form, Profile.
- Iterate in Stitch until the screens look right, then **export the code**
  (HTML/CSS) or copy to Figma. Save exports into
  `apps/fitness-app/stitch-exports/` (one folder per screen).

## Phase 2: Build with Claude Code (in this repo)

Give Claude Code this brief:

> Build the fitness app in `apps/fitness-app/` as a mobile-first PWA using the
> Stitch exports in `apps/fitness-app/stitch-exports/` as the visual source of
> truth. Follow CLAUDE.md, the chosen design/styles file, and the
> `mobile-native` and `animate` skills. Version 1 features: [list]. Use local
> storage first (no accounts) so I can try it on my phone, then we add
> login and a database.

Claude Code will:
1. Turn the static screens into reusable components and real navigation.
2. Add the logic (workout timer, logging sets, saving progress).
3. Make it installable on a phone (PWA manifest, icons, offline).
4. Add the motion layer per `ANIMATION-PLAYBOOK.md`.
5. Run it and screenshot it at phone size; then `/impeccable audit` and
   `break-ui` before handing over.
6. Later: accounts and database (e.g. Supabase), coach dashboard, payments
   (Stripe), and push reminders.

## Guardrails

- Health and fitness data is personal. Use proper login, privacy policy and
  consent before real clients use it, and never put client data in the repo.
- No invented testimonials, results or medical claims in the app or its
  store/landing page.
- Exercise programming content comes from the owner, not generated filler.
