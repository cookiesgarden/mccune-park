# McCune Park Pins

Pilot app for McCune Family Park (Eastvale): park ambassadors drop pins with photos on an aerial map; JCSD staff track each report (new → received → in progress → done), share ranger work sheets, and download the monthly Ambassador Submission Report.

- Static site: `index.html` (no build step). Deployed on Vercel.
- Backend: Supabase (Postgres functions + public `photos` storage bucket). The database setup script is kept out of this repo because it contains the access-link keys.
- Access: no sign-in. Each link carries a key (`/#k=...`) whose role (owner, staff, ambassador) is checked by the database functions.
