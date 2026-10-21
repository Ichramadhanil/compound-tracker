# Compound Tracker

Personal dashboard for a 20%-per-session compounding plan on a US stock portfolio
($154 start, Oct 19 → Dec 31, 2026, NYSE trading days only).

- Log the portfolio balance after each session; the page checks it against the
  20% target from your previous balance and against the plan schedule.
- Balances sync across devices through a private Supabase database. Each device
  is linked once with a secret sync link (QR code in "Sync & backup"); only a
  hash of that secret is stored, and the tables are closed to the public API.
  Nothing personal is stored in this repository.
- Every change is also kept in the browser first, so the page works offline and
  uploads when the connection is back.
- Settings (start capital, dates, daily %, holiday handling) are editable in the page.
