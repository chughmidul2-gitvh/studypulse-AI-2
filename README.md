# StudyPulse AI

**Problem statement: #4 – Open Innovation (Student Pain Points)**

## What it does
StudyPulse AI is a single-page web app that helps AKTU 1st-year engineering students prepare for exams. It brings study resources, active-recall practice, a syllabus progress tree, a focus timer and reminders together in one place, and nudges students back to studying when they go idle.

## Done / Left / Plan
**Done (works now)**
- Register / login (stored locally in the browser)
- Resource hub for AKTU 1st-year study material
- Active-recall practice cards
- Syllabus progression tree and retention analytics view
- 25-minute focus timer
- Study reminders with an on-screen alarm and snooze
- Inactivity guard ("Are you still studying?") and device-adaptive layout
- Voice prompts using the browser's speech synthesis

**Left (next 16 hours)**
- Email reminders (code is ready, needs the team's own EmailJS keys, kept out of the repo on purpose)
- Real backend storage instead of browser-only storage
- More subjects and PYQ content beyond the demo data

**Plan**
- Finish the left items in order: content, then backend, then email alerts.

## Architecture and why
- **Single HTML file (`index.html`)** with plain JavaScript: no build step, so anyone can open it and it deploys directly on GitHub Pages.
- **Tailwind CSS (CDN)** for fast, responsive styling on phones and laptops.
- **localStorage** for user data and reminders: no server needed for a demo and no personal data leaves the device.
- **EmailJS (optional)** for sending reminder emails from the browser without our own server. Keys are left empty in the repo.
- **Browser speech synthesis** for voice prompts: free, no API key.

## What we added
- Idle "Guardian" that warns the student and closes the session after inactivity, to reduce passive screen time.
- Device-adaptive layout so the app fits phone and desktop.
- Reminders that still fire when the app is opened late.

## Run it
Open `index.html` in a browser, or use the GitHub Pages link.

## Team
**Team: Mridul Chugh**

- Mridul Chugh
- Pranjal Pal
- Ashish Kumar
