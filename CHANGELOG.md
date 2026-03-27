# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [v1.0.1] - 2026-03-27

### Added
- Listing compliance metadata in `server.json`:
  - `tools` annotations with `readOnlyHint: true` for all exposed tools
  - `privacy_policies` including `https://aliceapp.ai/privacy-policy`

### Changed
- Bumped `server.json` version to `1.0.1`.
- Clarified README setup language to explain that the generated connection URL already includes the user's API key.
- Added a direct privacy policy link in the README "Privacy & Security" section.

## [v1.0.0] - 2026-03-23

### Added
- Initial public release of the Alice MCP Server.
- MCP server metadata and `streamable-http` remote configuration in `server.json`.
- Core tool surface for Alice recordings:
  - `search_recordings`
  - `get_transcript`
  - `get_recording_metadata`
  - `list_recent_recordings`
