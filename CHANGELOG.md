# Changelog

All notable changes to `phpstan-craftcms` will be documented in this file.

Updates should follow the [Keep a CHANGELOG](http://keepachangelog.com/) principles.

## [Unreleased](https://github.com/studio-stomp/phpstan-craftcms/compare/0.2.1...main)

### Added
- Add `roave/security-advisories` package

### Changed
- Moved actual extension code to `extension.neon` as `phpstan.neon` should be used for checking this package, not the consumer
- Add PHPStan as a dependency

### Removed
- Removed support for PHP 7.3

## [0.2.1](https://github.com/studio-stomp/phpstan-craftcms/compare/0.2.0...0.2.1) - 2021-05-13

### Changed
- Support PHP 8.0

## [0.2.0](https://github.com/studio-stomp/phpstan-craftcms/compare/0.1.1...0.2.0) - 2021-01-06
**Two big changes making it easier to get to level 2+ on a Craft CMS project**

### Added
- Dependabot

### Changed
- **Resolve configured attributes (Field / FieldLayout) on Elements**
    - Assume existence of compiled classes to resolve Field-based methods and attributes
    - TODO: add fallback to just checking project config yaml files (would be harder to get type information though)
    - TODO: allow changing location of compiled classes
- Stub `BaseYii` to resolve `$app` as Craft-namespaced Application
- Leave `paths` config directive to be implemented by project level

## [0.1.1](https://github.com/studio-stomp/phpstan-craftcms/compare/0.1.0...0.1.1) - 2020-08-27

## [0.1.0](https://github.com/studio-stomp/phpstan-craftcms/tree/0.1.0) - 2020-05-21

### Added
- Initial commit, based on the [PHP League Skeleton](https://github.com/thephpleague/skeleton)
