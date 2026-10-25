# ha-blueprints

Home Assistant blueprints for nashant's house.

| Blueprint | Import |
|---|---|
| Alarmo zone alarm | `blueprints/automation/alarmo_zone_alarm.yaml` |

## Branches

- `dev` — what `homeassistant-dev` runs. Change and test here first.
- `main` — what prod runs. Protected: changes arrive by PR from `dev`.

Each instance imports from its own branch, so its re-import button pulls
that branch:

- dev:  `https://github.com/nashant/ha-blueprints/blob/dev/blueprints/automation/<file>`
- prod: `https://github.com/nashant/ha-blueprints/blob/main/blueprints/automation/<file>`

Re-import overwrites the installed copy and reloads every automation using
it; an incompatible change breaks them. Breaking input changes get a new
file name rather than an in-place edit.
