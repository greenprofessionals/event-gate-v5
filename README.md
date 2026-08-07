# Event Gate V5

This is the separate gate-only module for Event Ticketing Platform V5.

It uses the same Apps Script endpoint as `event-ticketing-v5`, but role checks restrict Gate Staff to assigned active events.

## Gate Staff
- Select assigned active event.
- Scan QR from camera or photo.
- Enter serial manually.
- Search guest by name/phone/serial using a minimal data view.
- Check in valid tickets.
- See clear VALID / ALREADY CHECKED IN / REVOKED / NOT VALID results.

## Gate Supervisor
Includes Gate Staff rights plus:
- Undo accidental check-in with reason.
- Issue/check in walk-ins.
- View guest contact buttons when available: Email, WhatsApp, Text, Call.
- Authorized capacity override for walk-ins.

## Deployment
Copy `site-config.example.js` to `site-config.js`, paste the same V5 Apps Script `/exec` endpoint, and upload this whole folder to `event-gate-v5/` on GitHub Pages.
