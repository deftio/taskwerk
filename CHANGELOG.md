# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.7.13-dev] - 2025-07-25

### Added
- **AI Chat Context**: Conversations are now maintained across ask/agent commands
  - Project-specific contexts when inside a taskwerk project
  - Global named contexts for general use
  - `--context <name>` flag to use specific named contexts
  - `--new` flag to start fresh conversations
  - `--quiet` flag to hide context display
- **Search Command Alias**: `twrk search <term>` as shortcut for `twrk list --search <term>`
- **Enhanced Help**: Updated CLI help with chat context examples and better organization

### Changed
- Ask and Agent commands now maintain conversation history automatically
- Improved help text with more examples for search and split commands
- Added AI Chat Context section to README.md

### Fixed
- Test suite compatibility with chat management database migrations

## [0.3.10] - 2025-01-06

### Changed
- Consolidated v3 documentation from 10+ planning documents into 3 focused guides:
  - **v3-taskwerk-prd.md** - Product Requirements & Vision
  - **v3-cli-reference.md** - Complete CLI Reference  
  - **v3-implementation-guide.md** - Technical Implementation Guide
- Archived all planning and harmonization documents to `dev/archive/v3-planning/`
- Updated README.md to reference new v3 documentation structure

### Fixed
- Resolved terminology conflicts (use `active` not `in_progress`)
- Clarified command structure (subcommands not flat commands)
- Unified notes implementation approach (dual: field + table)

## Previous Versions

See git history for changes prior to v0.3.10.