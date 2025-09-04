# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.4.9](https://github.com/ratatui/kasuari/compare/v0.4.8...v0.4.9) - 2025-09-04

### Added

- always use `std` atomic types when using `--all-features` ([#33](https://github.com/ratatui/kasuari/pull/33))

## [0.4.8](https://github.com/ratatui/kasuari/compare/v0.4.7...v0.4.8) - 2025-09-04

### Other

- *(deps)* bump the rust-dependencies group across 1 directory with 2 updates ([#32](https://github.com/ratatui/kasuari/pull/32))
- add smoke tests for no_std targets ([#31](https://github.com/ratatui/kasuari/pull/31))
- use portable-atomic to allow use on targets without atomic instructions ([#30](https://github.com/ratatui/kasuari/pull/30))
- *(deps)* bump actions/checkout from 4 to 5 in the github-actions group ([#27](https://github.com/ratatui/kasuari/pull/27))
- *(deps)* bump the rust-dependencies group with 2 updates ([#28](https://github.com/ratatui/kasuari/pull/28))
- *(deps)* bump rstest from 0.25.0 to 0.26.1 in the rust-dependencies group ([#25](https://github.com/ratatui/kasuari/pull/25))
# Changelog

## [0.4.7](https://github.com/ratatui/kasuari/compare/v0.4.6...v0.4.7) - 2025-06-27

### Other

- *(gitignore)* add `.env` to `.gitignore` ([#22](https://github.com/ratatui/kasuari/pull/22))
- use variables directly in the `format!` string ([#23](https://github.com/ratatui/kasuari/pull/23))
- *(deps)* bump hashbrown from 0.15.3 to 0.15.4 in the rust-dependencies group ([#19](https://github.com/ratatui/kasuari/pull/19))
- fix for code scanning alert no. 1: Workflow does not contain permissions ([#20](https://github.com/ratatui/kasuari/pull/20))

## [0.4.6](https://github.com/ratatui/kasuari/compare/v0.4.5...v0.4.6) - 2025-05-08

### Added

- *(no_std)* option to disable `std` ([#16](https://github.com/ratatui/kasuari/pull/16))

## [0.4.5](https://github.com/ratatui/kasuari/compare/v0.4.4...v0.4.5) - 2025-05-06

### Other

- fix repo links joshka->ratatui org ([#14](https://github.com/ratatui/kasuari/pull/14))

## [0.4.4](https://github.com/ratatui/kasuari/compare/v0.4.3...v0.4.4) - 2025-05-06

### Other

- remove unused deps ([#12](https://github.com/ratatui/kasuari/pull/12))

## [0.4.3](https://github.com/ratatui/kasuari/compare/v0.4.2...v0.4.3) - 2025-04-04

### Other

- use the same formatting as ratatui ([#9](https://github.com/ratatui/kasuari/pull/9))

## [0.4.2](https://github.com/ratatui/kasuari/compare/v0.4.1...v0.4.2) - 2025-04-04

### Other

- fix release-plz check to ratatui-org
- move to ratatui github org ([#7](https://github.com/ratatui/kasuari/pull/7))
- configure dependabot
- add coverage

## [0.4.1](https://github.com/ratatui/kasuari/compare/v0.4.0...v0.4.1) - 2025-04-04

### Other

- fix build badge

## [0.4.0](https://github.com/ratatui/kasuari/compare/v0.4.0-alpha.2...v0.4.0) - 2025-04-04

### Added

- add const methods for Strength ops
- make Strength new() and create() const

## [0.4.0-alpha.2](https://github.com/ratatui/kasuari/compare/v0.4.0-alpha.1...v0.4.0-alpha.2) - 2025-04-04

### Added

- make the crate `no_std` ([#2](https://github.com/ratatui/kasuari/pull/2))

### Fixed

- clippy lints
- doc tests

### Other

- add release-plz automation
- rename ci workflow
- tweak cargo.toml, unignore cargo.lock
- add simple ci workflow

## Kasuari 0.4.0-alpha.1

This release is a fork of the library under a new name, `Kasuari`. The name change is to avoid confusion
with the original `Cassowary-rs` library, which has been unmaintained since 2018. The name `Kasuari` is
the Indonesian name for the Cassowary bird.

- Initial Kasuari release
- Update to Rust 2021 edition
- Update docs
- Reformat code
- Cleanup lints
- Move code to appropriate modules
- Add `Debug` implementations for various types
- Implement Error for errors and provide better error messages
- Add error source to InternalSolverError for better debugging
- Add tests
- Spell optimise with US english (optimize)
- Make Strength a newtype instead of f64
- Pass constrains by value instead of reference

## Casssowary 0.3.0

- Various fixes (PR #4) from @christolliday.
  > Main breaking change is that variables no longer silently initialise to zero and will report
  their initial value in the first call to `fetch_changes`, also `has_edit_variable` now takes
  `&self` instead of `&mut self`.

## Casssowary 0.2.1

- Fixed crash under certain use cases. See PR #1 (Thanks @christolliday!).

## Casssowary 0.2.0

- Changed API to only report changes to the values of variables. This allows for more efficient use
  of the library in typical applications.

## Casssowary  0.1

Initial release
