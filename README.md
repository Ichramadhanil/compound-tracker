# Road to $1M — Compound Tracker

Personal dashboard for growing a US stock portfolio to $1,000,000 by Dec 31, 2026
(NYSE trading days only).

- **Dynamic daily target.** Each session's target % is recalculated from the current
  balance: (goal ÷ balance)^(1 ÷ sessions left) − 1. Miss a day and the target rises;
  beat it and the target falls.
- **Input = daily % gain**, plus win/lost trade counts. The balance is calculated
  automatically by compounding the daily % from the starting capital.
- **Statistics:** on-track status vs. the ideal path, required % per day, pace and
  $1M ETA, what-if table, green/red days, drawdown, win rate and more.
- **Journal:** per-session notes (pattern recognized, why trades lost, why trades won,
  with #tags). Each month gets an automatic in-page summary, and on the 1st of every
  month Claude writes a review of the previous month's notes.
- **Sync:** data syncs across devices through a private Supabase database. Each device
  is linked once with a secret sync link (QR code in "Sync & backup"); only a hash of
  that secret is stored, and the tables are closed to the public API. Nothing personal
  is stored in this repository. Changes are kept in the browser first, so it works offline.
