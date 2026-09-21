# Contributing to Foldrone Play

Thank you for helping improve Foldrone Play.

## Before contributing

Read:

- [README.md](README.md)
- [SECURITY.md](SECURITY.md)
- [CHANGELOG.md](CHANGELOG.md)

## Development principles

### Preserve playback stability
A visual improvement must not silently break playback.

### Preserve universal behavior
Prefer responsive and capability-based solutions over device-specific assumptions.

### Keep the Media Core modular
Optional capabilities should not make core playback unusable when unavailable.

### No secrets
Never commit API keys, tokens, passwords, certificates, provider credentials or secret `.env` files.

## Pull requests

Explain:

- What changed
- Why it changed
- Devices/layouts tested
- Playback behavior affected
- Security implications, if any

Small, focused changes are preferred.
