# renovate-config

Shared [Renovate preset](https://docs.renovatebot.com/config-presets/) for `jamesholland-uk` repos.

Each repo's `renovate.json` extends it:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["local>jamesholland-uk/renovate-config"]
}
```

Repo-specific rules (custom managers, package schedules, looser automerge) go in that repo's
`renovate.json` after the `extends`. They are applied on top of this preset.

This repo is private, so the Mend Renovate app must have access to it.

When you learn something or improve the policy here (e.g. `internalChecksFilter: strict`), apply it to
`obsidian-desert-ops/renovate-config` too, if it fits there. That repo deliberately doesn't refer back to this one.
