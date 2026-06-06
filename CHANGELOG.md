# Changelog

All notable changes to this repository are tracked here.

## 0.1.0 - 2026-06-06

### Added

- Add explicit skill operating modes: `plan_only`, `generate`, `edit`, and `save`.
- Add a pre-generation image spec contract before `image_gen` calls.
- Add deterministic save rules for slugged folders, sequential filenames, collision suffixes, and absolute-path handoffs.
- Add a zero-dependency repository validator exposed through `npm test`.
- Add copied-skill version tracking through `ian-xiaohei-illustrations/VERSION`.

### Changed

- Expand prompt and QA references so generation, editing, and saving rules are visible to future agents.
- Document the validation workflow in the README.
