# My standard renovate config

Shared [Renovate config presets](https://docs.renovatebot.com/config-presets/) for easier use across my projects.

## Usage

To re-use the default config, add this to the `renovate.json`:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>LBBO/renovate-config"]
}
```

To also enable automerge of non-major updates if all tests pass, add the following:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>LBBO/renovate-config",
    "github>LBBO/renovate-config:automerge-non-major"
  ]
}
```

