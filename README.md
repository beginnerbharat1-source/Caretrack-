# CareTrack 2.0 — real full-stack MVP

CareTrack is now a real server-backed web application rather than a browser-local prototype.

## Included
- Email/password account creation and login
- Per-user data isolation
- SQLite persistent database
- Server-side storage for readings, medicines and profile
- Session authentication using HttpOnly cookies
- Add/delete readings and medicine reminders
- Mark medicine reminders taken for the current day
- Existing CareTrack dashboard, trends and doctor report UI

## Run locally
1. Install Node.js 20+
2. `npm install`
3. `npm start`
4. Open `http://localhost:3000`

The database is created at `data/caretrack.db`.

## Deploy
GitHub Pages cannot run this backend. Deploy this project to a Node-capable host such as Render, Railway, Fly.io, or your own server. Set `NODE_ENV=production` and attach persistent storage for the `data` directory.

For real clinical/patient use, this MVP still needs a security/compliance review, HTTPS, backups, audit logging, access/role controls, consent/privacy workflows and applicable Indian healthcare/data requirements before storing sensitive patient records.
