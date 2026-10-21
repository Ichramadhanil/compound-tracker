# Compound Tracker

Personal dashboard for a 20%-per-session compounding plan on a US stock portfolio
($154 start, Oct 19 → Dec 31, 2026, NYSE trading days only).

- Log the portfolio balance after each session; the page checks it against the
  20% target from your previous balance and against the plan schedule.
- Everything runs in the browser. Balances are saved in this browser's local
  storage only, never in this repository. Use "Export backup" to move them to
  another device.
- Settings (start capital, dates, daily %, holiday handling) are editable in the page.
