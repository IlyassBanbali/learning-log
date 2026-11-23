# Today I learned

- 2026-11-23: WSL2 gets half of host RAM by default; `.wslconfig` raises the limit and `wsl --shutdown` applies it.
- 2026-11-23: Two Sum — a hash map of seen values turns the O(n²) pair search into one O(n) pass.
- 2026-11-23: SQL `BETWEEN a AND b` includes both ends; `NOT BETWEEN` keeps rows outside the range; NULLs match neither.
- 2026-11-24: Contains Duplicate — a set gives O(1) average membership checks; O(n) time, O(n) space, stop at the first repeat. Use a set for "seen?", a dict when you need a stored value.
- 2026-11-24: SQLBolt 3–4 — text filters (LIKE, IN), DISTINCT, ORDER BY, LIMIT/OFFSET. Anki set up with 20+ cards.
- 2026-11-24: Missing Semester 01 — the shell finds programs via PATH; > overwrites, >> appends, < feeds input, | chains programs.
- 2026-11-24: Missing Semester 01 exercises done — shebang + chmod +x to run a script; ./script runs it via the shebang, sh script runs it via sh directly.
- 2026-11-24: Valid Anagram — count up for s, down for t, then all(v == 0); summing counts is not enough because +1/-1 on different letters cancel. Return the boolean directly, never if cond: return True.
