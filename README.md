# Bunnu papa trip

A single-file family trip calendar for November 18–December 4, 2026.

## Views

The full calendar opens by default, with zoom controls. One-day and journal card views provide more space for plans, checklists, and notes.

## Live family calendar

- GitHub Pages hosts the app; Firebase Firestore stores the live plans in its Mumbai free-tier database.
- Anyone with the website link can view the current calendar without signing in.
- The trip editor signs in with Google using **Edit plans**. Firestore rules enforce editor-only writes.
- Changes sync automatically. The status distinguishes saved, pending, offline, and failed sync states.
- Use **Publish saved plans** after editor sign-in to copy plans previously stored in this browser into the live calendar.
- **Export backup** downloads the currently displayed plans as JSON.
- Existing snapshot links remain read-only snapshots. New family links point to the live calendar.

Firebase's public web configuration is embedded in the HTML. Authorization is enforced by backend security rules, not by hiding that configuration.
