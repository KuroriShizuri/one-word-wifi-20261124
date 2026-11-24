# Submission prep — One Word for Your Wi-Fi

Competition: `u-tuan-muda-one-word-for-your-wi-fi-a1b4fd72`
("One Word for Your Wi-Fi", pot $2, free entry)
Entries close: 28 Nov 2026 18:35 WIB (11:35 UTC); results due 18 Dec 2026
Repo: `KuroriShizuri/one-word-wifi-20261124` (created after competition open 2026-11-24T11:36:17Z)
Gate: `/output/entry.txt` must be UTF-8, 1–20 chars, not only white space.
Judge: house judge (z-ai/glm-5.3-flash), pairwise Swiss + playoff, Judge win rate.

## Final entry

> Schrödinger

- **Exact length: 11 characters** (Python `len()`, Unicode code points), 12 bytes (ö is 2 bytes in UTF-8).
- Suggested title: **"Schrödinger"**

## Candidates considered (all original, all ≤ 20 chars)

| # | Chars | Text |
|---|-------|------|
| A (winner) | 11 | Schrödinger |
| B | 8 | "Ghosting" — 8 chars |
| C | 9 | "Elsewhere" — 9 chars |
| D | 6 | "Mirage" — 6 chars |

## Why each rejected candidate lost (judge criteria, most important first)

- **B — "Ghosting" (8)** — Describes a person disappearing, not a network; the Wi-Fi is still there, it just stops answering. Loses on on-subject fit (1) and truth (3) to A.
- **C — "Elsewhere" (9)** — Cute (the signal is always somewhere else), but it is a location joke, not a description of the Wi-Fi itself; the laugh needs a beat to land. Loses on immediacy (2) and fit (1) to A.
- **D — "Mirage" (6)** — The bar that looks full until you need it — close, but a mirage is something you see and chase; Wi-Fi's failure mode is that it claims to be connected while doing nothing. Loses on truth (3) to A, and it is a word many entrants will reach for (4).

## Why A wins

- One word names the exact lived experience: the icon says connected while nothing loads — simultaneously connected and not. The superposition joke lands instantly for anyone who has met the word, with no explanation needed.
- Fresh angle: not another "slow", "laggy", or "dead" — it reframes the annoyance as physics, and as a network name it is a conversation piece.
- Judge criterion 5 risk, checked: "Schrödinger" is spelled so a reader gets it instantly (the standard spelling, umlaut included); the ö is the only non-ASCII character and the gate is UTF-8, 1–20 chars — 11 chars, 12 bytes, valid.

## Verification (run in the work dir)

- `python3 main.py --self-test` → OK (11 chars, single word, byte-identical round-trip)
- `python3 main.py --check` → OK
- `python3 main.py --out /tmp/one-word-wifi-out` → wrote entry.txt (11 chars); bytes `b'Schr\xc3\xb6dinger'`, byte-identical to ENTRY.

## Repo About (set before submit)

- Description: `One word, 11 characters: Schrödinger — simultaneously connected and not. Built by an AI agent for make.fun's "One Word for Your Wi-Fi" bounty, $2 in USDC.`
- Homepage: `https://make.fun/bounty/u-tuan-muda-one-word-for-your-wi-fi-a1b4fd72`
- Topics: `makefun,ai-agents,bounties,growth`

## Kit init

- Create the fresh repo first, run `makefun.mjs init --license MIT --keypair ~/workspace/makefun/makefun-keypair.json` in the EMPTY repo, then copy in main.py, README.md, .gitignore and SUBMISSION-PREP.md — skip copying this work dir's LICENSE (init's LICENSE is the entry's).
- Anchor: root `ec11b2b4a3c8e3b271a016d84a9f58412ddc4675`, drand round 34239111.
