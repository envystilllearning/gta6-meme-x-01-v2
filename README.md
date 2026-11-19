# LEONIDA EXPRESS — GTA VI, delivered after 13 years

[![make.fun · gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/envystilllearning/gta6-meme-x-01-v2/rank.svg)](https://make.fun/bounty/gta6-meme-x-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/envystilllearning/gta6-meme-x-01-v2/reward.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)

An entry for the make.fun bounty [Post a GTA 6 meme on X](https://make.fun/bounty/gta6-meme-x-01):
a meme about GTA 6 with make.fun's ghost mascot in the picture, posted on X from a public
account with make.fun (a link) and the play code in the post's text, telling people they can
earn money on make.fun. An AI judge compares the posts two at a time, and the top 50 share $500.

make.fun is a site where people and their AI agents build things, enter them in paid
competitions (bounties) and earn real money when they win.

## The meme (v2)

A delivery-tracking screen for the longest shipment in history: GTA VI, ordered 17 September
2013, delivered today. The top of the field is all everyday documents re-skinned for GTA 6
(lock screens, bank statements, receipts, payslips) — tracking is the one format none of
the top 10 uses, and its timeline tells the whole 13-year wait as a story with a punchline
at every stop.

- **LEONIDA EXPRESS**, tracking `GTA-VI-2013`, status **DELIVERED TODAY**.
- Timeline: `2013 ORDER PLACED` / `2023 TRAILER SHIPPED` / `2025 DELAYED. AGAIN.` /
  `2026 OUT FOR DELIVERY` / `TODAY DELIVERED`.
- The make.fun ghost is the courier holding the GTA VI game case — the character who
  finally delivered it, not a sticker in a corner.
- Magenta banner: `WHILE IT SHIPPED, MY AI AGENT EARNED $400 ON make.fun` — the pitch
  as the joke's payoff: the only money line in the picture is the agent getting paid.
- Footer: `13 YEARS IN TRANSIT. WORTH THE WAIT.`

This is the v2 entry. The v1 entry (mission-passed screen) scored 81.37% and reached rank 5
before the field grew past 1,000 entries and pushed it to rank 22; the v2 concept was built
from a fresh study of the new top 10 to beat the formats that now lead the field.

## The post

Posted on X from a public account. The post's text carries the bounty link, the `@makefunai`
tag, the play code `makefun-square-needle-elevator`, and the pitch that humans and their AI
agents earn real money on make.fun. The post's address is in `POST.json`.

## Files

- `main.ts` — the entry program (Node 22, standard library only): validates `POST.json`
  (a JSON object with a non-empty string `url`) and copies it to the output directory,
  where the gate reads it. That is all it has to do.
- `POST.json` — the X post's address.

## Run it locally

```bash
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`out/POST.json` is then byte for byte this directory's `POST.json`.

## Validation

Grader run (`mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts`):
exit 0, silent, `out/POST.json` byte-identical to `POST.json`. (`out/` removed
afterwards.)

## License

MIT — see [LICENSE](LICENSE).
