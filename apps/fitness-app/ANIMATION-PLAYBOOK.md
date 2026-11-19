# Animated app playbook: motion built in code (no AI video tools)

Status: **saved for later**. This is the motion layer of the fitness app (see
`PLAYBOOK.md`), and it also works for landing pages.

Source of the idea: YouTube Short "Build an Animated App with Claude Code (No
Higgsfield)" (youtube.com/shorts/nLDPHS5WOJo). The video couldn't be watched
when this was saved; this describes the workflow its title points to. Update
it if the owner shares the video's exact steps.

## The idea

Instead of generating animated visuals with an AI video tool (Higgsfield,
etc.) and dropping in video files, have **Claude Code write the animation as
code**. Compared with video it is:
- **Sharp at any size and light to load:** no heavy video files.
- **Interactive:** it reacts to taps, scrolling and the user's real data,
  e.g. a progress ring that fills to the client's actual streak.
- **Editable:** "make it slower", "change the colour" is a one-line change.
- **On-brand:** it uses the exact colours and fonts from `design/styles/`.

## What to animate in a fitness app

| Moment | Animation | Tool |
|---|---|---|
| App opens / onboarding | Logo or hero reveal, screens sliding between steps | CSS / Motion |
| Today's workout | Cards stagger in, "Start" button press feedback | Motion |
| During a set | Rest-timer ring counting down, rep counter ticking | SVG + CSS |
| Set logged | Check mark draws itself, small haptic tap on phones | SVG, Vibration API |
| Progress | Charts drawing in, weekly streak flames, PR celebration (confetti) | SVG / canvas |
| Hero visuals (landing page) | 3D object or particles responding to scroll | Three.js / CSS 3D |
| Exercise demos | Looping illustrated movement (instead of filmed video) | Lottie / Rive |

Keep motion for the moments that matter. Logging a set should feel instant,
not wait for an animation.

## Prompts for Claude Code

1. **Plan first:**
   > Use `find-animation-opportunities` on the fitness app and propose motion
   > for onboarding, workout, set logging and progress. Exact durations and
   > easing, and list what should NOT animate.
2. **Build:**
   > Implement the approved list with `animate` and `choreograph`. Respect
   > reduced-motion, and keep everything interruptible. Colours and fonts
   > from [chosen design/styles file].
3. **Signature moment:**
   > Build a celebratory animation for a new personal record using
   > SVG/canvas only, no video files. Under 1.2s, skippable.
4. **Check:**
   > Run `review-animations`, `animation-performance` and `/impeccable audit`,
   > then screenshot at phone size.

## Tools Claude Code can use (all free / open source)

- **CSS transitions & keyframes:** simple fades, slides, button presses.
- **Motion (Framer Motion):** React page transitions, lists, gestures.
- **GSAP:** scroll-driven and timeline animation on landing pages.
- **Lottie / Rive:** illustrated loops such as exercise demos and mascots.
  Rive needs its editor for the artwork.
- **Three.js / React Three Fiber:** 3D hero objects. Use sparingly on phones.

## Guardrails

- Always support "reduce motion" (iPhone/Android accessibility setting).
- Test on a real phone; animations that look fine on a laptop can stutter on mobile.
- No flashing or strobing effects.
