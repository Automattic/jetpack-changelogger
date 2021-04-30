# Changelog
All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.0-alpha] - unreleased

This is an alpha version! The changes listed here are not final.

### Deprecated
- Changelogger `Config::setOutput()` is no longer needed. Config will throw a ConfigException instead of printing an error.

### Fixed
- If composer.json is not present in the current directory, check parents and ask if the parent should be used (like composer does).

## [1.1.2] - 2021-04-08
### Fixed
- Don't insert extra newlines if a subsection has no non-empty entries.

## [1.1.1] - 2021-03-30
### Changed
- Build infrastructure changes, nothing affecting the package itself.

## [1.1.0] - 2021-03-22
### Added
- Allow "unreleased" as the date for a changelog entry.
- Enable GitHub action for auto-tagging releases from monorepo pushes.

### Changed
- Branch-alias dev-master rather than dev-monorepo, as we're removing the hack.

### Fixed
- Use `composer update` rather than `install` in scripts, as composer.lock isn't checked in.

## 1.0.0 - 2021-03-08
### Added
- Initial version.

[1.2.0-alpha]: https://github.com/Automattic/jetpack-changelogger/compare/1.1.2...1.2.0-alpha
[1.1.2]: https://github.com/Automattic/jetpack-changelogger/compare/1.1.1...1.1.2
[1.1.1]: https://github.com/Automattic/jetpack-changelogger/compare/1.1.0...1.1.1
[1.1.0]: https://github.com/Automattic/jetpack-changelogger/compare/1.0.0...1.1.0
