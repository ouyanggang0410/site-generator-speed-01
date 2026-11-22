# site-generator-speed-01

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/ouyanggang0410/site-generator-speed-01/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/ouyanggang0410/site-generator-speed-01/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A fast static site generator whose output is byte-identical to makefun-site 1.0.0's build for every input. Written from the makefun-site dialect spec and verified against the kit's practice set and scorer (3/3 cases) plus three freshly drawn generator instances (9/9 cases).

Speed comes from structure, not shortcuts: plain text runs are copied as slices instead of escaped one character at a time, Markdown blocks render straight to HTML without an intermediate token tree, slugs are cached and skip Unicode normalisation on pure-ASCII text, word counting never builds a match array, and each page's card is built once.

## Run it

```sh
node main.ts
```

`main.ts` reads every case from `/input/cases.json` (or `$MAKEFUN_INPUT_DIR`) and writes `/output/answers.json` (or `$MAKEFUN_OUTPUT_DIR`). `solve.js` exports `run(input)`, the build for one case.

---

<sub>Entered on [make.fun](https://make.fun/?ref=qhmde06g&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
