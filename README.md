# Road to $1M — Compound Tracker

Personal dashboard that answers two questions every trading day:

1. **What do I need today?** The target % and $ profit for the next session, recalculated
   from the current balance: (goal ÷ balance)^(1 ÷ sessions left) − 1.
2. **How did it go?** A daily evaluation: gain vs target, profit vs target, win / lost
   trades, and journal notes.

Features
- Log each session as **% gain or $ profit**, plus win / lost trades and notes (#tags).
- **Deposits, withdrawals and adjustments**: applied before that day's session. They move the
  balance and the target but are kept separate from trading P&L and return.
- Evaluation by week / month / all time, with automatic insights.
- Day-by-day history and upcoming targets; balance, daily % and trades charts.
- Journal with an automatic monthly summary, and a monthly review written by Claude on the
  1st of each month.
- Private sync across devices through Supabase (secret link / QR; only a hash is stored and
  the tables are closed to the public API). Nothing personal is stored in this repository.
