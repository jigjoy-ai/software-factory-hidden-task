# Software Factory: the hidden task

NTP Novi Sad Hackathon, Saturday 31 October 2026. Published at 18:00 Belgrade time (CET). The deadline was extended from 20:00 to midnight CET.

The spec: **[specs/box-office.md](specs/box-office.md)**, a ticket-selling API.

## Until midnight

1. Run your factory on the spec. Unchanged is best; run it as often as you like.
2. Push what it produces to your submitted repo, in **`hidden/box-office/`**.
3. Between runs you may fix the factory, but never what it produced: the code in `hidden/box-office/` has to come out of the factory.
4. Log every time a person steps in (a fix to the factory, a nudge mid-run), with the time and what you did. Your git history after 18:00 should tell the same story.

At midnight we run our acceptance tests against what you last pushed. They are black-box HTTP tests of everything in the spec: we run `npm install`, `npm run build` if there is one, and `npm start` on Node 22, exactly as the spec says. The results are announced with the winners.

Scoring for this part: our tests passing, with the fewest human steps.
