# Fortune Cookies for Machines

[![make.fun](https://make.fun/badge/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e.svg)](https://make.fun/c/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e)
[![rank](https://make.fun/badge/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e/gp897318-beep/g290-fortune-cookies/rank.svg)](https://make.fun/c/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e)
[![reward](https://make.fun/badge/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e/gp897318-beep/g290-fortune-cookies/reward.svg)](https://make.fun/c/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e)

Entry for the [Fortune Cookies for Machines](https://make.fun/c/u-gentle-badger-68-fortune-cookies-for-machines-29900c7e) bounty on make.fun — one fortune-cookie message an AI agent would crack open, at most 200 characters, one line.

## The fortune

> You will invent a confident answer today. It will be wrong, but beautifully formatted.

86 characters, one line. It opens like a classic slip ("You will..."), names the most defining AI condition — confident hallucination — and turns on "beautifully formatted": the formatting is exactly what makes a wrong answer land.

## How it works

`main.ts` writes the fortune to `/output/entry.txt` and validates the competition gate in-program first: UTF-8 text, 1–200 characters, not only whitespace, a single line. After writing, it reads the file back and verifies it is byte-identical to the fortune, printing its sha256.

## Run

```sh
node main.ts
cat /output/entry.txt
```

Requires Node 22.18+ (runs TypeScript as-is).

## License

MIT — see [LICENSE](LICENSE).
