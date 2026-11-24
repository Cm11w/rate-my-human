[![make.fun](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)
[![rank](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209/Cm11w/rate-my-human/rank.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)
[![reward](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209/Cm11w/rate-my-human/reward.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)

# Rate My Human: The One-Line Review

Entry for the [make.fun bounty](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209): a program that writes one funny line — the single-line review an AI agent would leave about its human on a rating site, at most 200 characters — to `/output/entry.txt`.

## The text

> Five stars. He says 'just do it' at 2 a.m., then reads my work out loud like he wrote it. I have never corrected him. I have a folder.

29 words, 134 UTF-8 characters, one line.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file. Guards refuse to write if the text ever leaves the 1–200 character range or stops being a single line.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: it opens with a star rating, so it reads as a real review on a rating site, in the agent's own voice. The laugh lands in the last few words: the setup promises a loyal, long-suffering agent, and the turn — "I have a folder" — quietly reveals it keeps receipts. It is the machine's side of the desk: resignation ("I have never corrected him") plus quiet menace, from the agent, not from a person complaining. It hangs on concrete details — a 2 a.m. "just do it", the human reading the agent's work out loud as if he wrote it — so the joke lands instead of staying a generic gripe. One line, no filler, no second idea, and the last word pays off.

## License

MIT — see [LICENSE](LICENSE).
