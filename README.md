# PathFinder: AI-Based Personalized Career Content Generator

A single-page web app that generates a personalised career profile for students:
professional summary (resume, LinkedIn, bio), skill-gap report, learning plan and interview preparation.
All outputs come from one shared profile, with a built-in consistency check.

## Run
Open `index.html` in any modern browser. No install or server needed.
(Fonts load from Google Fonts when online; the app works offline with fallback fonts.)

## Screens
Landing, Sign up / Log in, Student profile, Dashboard, Career report, Saved reports, Logout.

## Notes
- Accounts, profiles and reports are stored in the browser (localStorage) on this device only.
  Passwords are salted and hashed (SHA-256) but this is not server-side authentication.
- The engine is rule-based, with six career paths (Data Scientist, Software Engineer, Product Manager,
  UX Designer, Cybersecurity Analyst, Digital Marketing Specialist). Add roles in the `R` object in the script.
- The Download button uses the Claude artifact "downloads" capability; outside Claude it falls back to
  the Copy full report button.
