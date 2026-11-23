# 第二季产品周赛｜阅读 04 文献智能问答 Skill｜标准题目与评分文档

Bohrium Playground Period 4 submission — challenge `challenge-15c85674` (track: `literature-reading`).

This repository holds the complete skill package for the challenge: the skill
definition, its executable entry point and all supporting scripts. No precomputed
answers, private data or credentials are included.

## Skill

- Name: `literature-qa-evidence`
- Summary: Use when a case asks questions about one paper and every answer must cite paragraph-level evidence from the supplied material.

## Contents

| File |
|------|
| `SKILL.md` |
| `scripts/run_skill.py` |
| `README.md` |

## How to run

```bash
python scripts/run_skill.py --case /input/case.json --output /app/output/result.json
```

The entry point is `SKILL.md`; input/output contracts, error handling and a minimal
usage example are documented there.

## Notes

- Pure Python standard library; no network access required.
- The result JSON keeps the input case id, the main results, per-item evidence,
  a run status and an uncertainty section.
