# LoopIn: a lead CRM for a real estate team
- One static page, `index.html`. It reads and writes a Supabase database. There is no build step.
- Who can see or change a lead is enforced by Supabase row-level security, not by this page.
- The Supabase publishable key in `index.html` is public by design. It grants nothing without a signed-in team member.
- Sign-in is Google only. A Google account that is not on the team sees nothing. Host it on GitHub Pages.
