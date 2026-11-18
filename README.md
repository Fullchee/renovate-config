# renovate-config

Shared [Renovate](https://docs.renovatebot.com/) preset for Fullchee's personal projects.

## Use it

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>Fullchee/renovate-config"]
}
```

## What it sets

- **Schedule**: Mondays before 9am, Toronto time, with at most 5 open PRs.
- **Release age**: updates wait 5 days, matching the global bun `minimumReleaseAge`, and stay hidden until then.
- **Labels**: PRs and the Dependency Dashboard get `dependencies`, so `/triage` skips the dashboard.
- **Dashboard**: pinned to the top of Issues.

A repo overrides any of these in its own `renovate.json`.
