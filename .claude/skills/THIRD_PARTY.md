# Third-party skills

Vendored from GitHub. To update, re-copy from the upstream repo.

| Skills | Source | Commit | License |
|---|---|---|---|
| `graphify` | https://github.com/Graphify-Labs/graphify (installed with `graphify install --project`, CLI from PyPI `graphifyy`) | b582ad4 | Apache-2.0 / MIT |
| `ponytail`, `ponytail-*` (6) | https://github.com/DietrichGebert/ponytail (`skills/`) | 96608e0 | MIT |
| `omni-*`, `cli-*`, `config-codex-cli` (45) | https://github.com/cheaper-inference/OmniRoute (`skills/`, its copy of ponytail skipped) | 3712be0d | MIT |

Notes:
- graphify's skill and hooks in `.claude/settings.json` need the `graphify` CLI: `uv tool install graphifyy`.
- OmniRoute skills drive an OmniRoute server/CLI (`npm i -g omniroute`); they do nothing without one running.
- Ponytail's always-on hooks (level persistence, subagent injection) come only with the plugin:
  `/plugin marketplace add DietrichGebert/ponytail` then `/plugin install ponytail@ponytail`.
