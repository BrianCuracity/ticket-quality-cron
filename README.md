# ticket-quality-cron

Pings the Curacity ticket-quality scanner every 5 minutes so edited Backlog
tickets get re-evaluated automatically. The endpoint requires a secret
(stored in this repo's Actions secrets as `WEBHOOK_SECRET`), so the workflow
being public exposes nothing sensitive.

Note: GitHub disables scheduled workflows after 60 days without repo activity —
GitHub emails a one-click "keep workflow active" link before doing so.
