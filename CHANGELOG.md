# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/).

## [Unreleased]

## [1.13.0] - 2023-02-27
### Added
- Support Laravel 9-10

### Removed
- Some older versions

## [1.12.0] - 2021-03-07
### Added
- A check that we are not on the callback route to prevent infinite looping in case the middleware is added globally
- Logout method to Guard

## [1.11.0] - 2021-03-06
### Added
- Laravel 8 / PHP 8 support

### Changed
- Use GitHub actions instead of Travis

### Removed
- Laravel 5 / PHP <= 7.2 support

## [1.10.0] - 2020-05-12
### Added
- Laravel 7 support
- PHP 7.4 coverage

## [1.9.0] - 2019-09-23
### Added
- Laravel 6 support

### Removed
- Laravel 5.4 / PHP 5.6 support

## [1.8.0] - 2019-06-01
### Added
- Alternative middleware that only checks but doesn't redirect if not logged
- PHP 7.3 Travis coverage

## [1.7.1] - 2019-03-23
### Fixed
- No longer attempt refresh_token grant without token
- Handle errors during refresh_token (same as invalid access-token -> Redirect to IP authorize)

## [1.7.0] - 2019-03-10
### Added
- Laravel 5.8 support

## [1.6.0] - 2018-12-30
### Added
- Possibility to specify an "AuthWrapperFactory" allowing custom creation of the User object

## [1.5.0] - 2018-11-03
### Added
- Laravel 5.7 support

### Changed
- Tests: Assign the middleware as route-middleware

### Fixed
- Readme: Config publish command quotes (otherwise would need to use `\\` in namespace)

## [1.4.0] - 2018-04-19
### Added
- Laravel 5.6 support

### Fixed
- Readme: composer require package name

## [1.3.0] - 2017-09-19
### Added
- Laravel 5.5 support
- Package Auto-Discovery

### Changed
- Travis build matrix
- Improved dependency version constraints
- Allow `league/oauth2-client` also at v1 - even though I don't recommend it a short test showed no problems/incompatibilities

### Fixed
- PHP 5.6 install stuck because of (loose) testbench constraints

## [1.2.0] - 2017-06-29
### Added
- `Auth`-driver *viaRequest* & `Authenticatable` wrapper

## [1.1.0] - 2017-05-25
### Added
- Configuration option to specify a custom OAuth2 provider class

## 1.0.0 - 2017-05-21
### Added
- Basic Project setup
- OAuth2 client middleware & callback
- Keeps token in session
- Refreshes expired tokens
- (Cached) resource owner info

[Unreleased]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.12.0...HEAD
[1.12.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.11.0...v1.12.0
[1.11.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.10.0...v1.11.0
[1.10.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.9.0...v1.10.0
[1.9.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.8.0...v1.9.0
[1.8.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.7.1...v1.8.0
[1.7.1]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.7.0...v1.7.1
[1.7.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.6.0...v1.7.0
[1.6.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.5.0...v1.6.0
[1.5.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.4.0...v1.5.0
[1.4.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/kronthto/laravel-oauth2-login/compare/v1.0.0...v1.1.0
