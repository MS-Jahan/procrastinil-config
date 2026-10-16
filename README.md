# procrastinil-config

Public, NON-SECRET runtime configuration for the ProcrastiNil app.

- `config.json` — tunable values the app reads at start (feature modes, VAD thresholds, grace limits, caps).
- `config.json.sig` — ed25519 detached signature (base64) over the exact bytes of `config.json`. The app ignores a config whose signature does not verify.

Never put secrets here. Anyone can read this repo.
