# Archive

Content that is **no longer part of the active plan**. Nothing in this folder should be
treated as current. The single source of truth for the plan is the top-level
[README.md](../README.md).

-----

## Dropped Tracks

| File | Was | Dropped Because |
|------|-----|-----------------|
| `track-12-python-advanced.md` | Python Advanced (AST, async) — 6 weeks | The architect reviews Python rather than writing advanced Python. Semgrep rule authoring, the one genuinely relevant piece, is already covered in Track 9. Async Python is not needed to direct Claude Code. |
| `track-13-javascript.md` | JavaScript/TypeScript — 14 weeks | Not on the critical path for AI red teaming. The one security-relevant piece — insecure handling of LLM output (OWASP LLM02) — was salvaged into Track 10 rather than left behind a 14-week JavaScript prerequisite. |

Both were previously staged as an "optional Part V" spanning Weeks 44-62. That framing made
the plan read as 63 weeks when the real commitment is 44. The drop was already documented in
[future-technical-reading.md](../future-technical-reading.md) under "Dropped from Plan
(Track 12 & 13)"; moving these files here finishes that decision.

**If your needs change:** see `future-technical-reading.md` for what to read instead, and for
the five JavaScript books you own that are no longer mapped to any track.
