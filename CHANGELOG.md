# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased](https://github.com/HubSpot/hubspot-php/compare/v2.0.7...v2)

## [2.0.7]

### Fixed
- Files::update

## [2.0.6]

### Fixed
- ContactProperties::updateGroup

## [2.0.5]

### Changed
- removing list contacts by email address
- minor changes

## [2.0.3]

### Added
- Line Items Resource
- Products Resource
- Object Properties Resource

### Changed
- Up php version to 7.0
- Update Ecommerce Bridge to v2
- Update Hub DB to v2
- Update Form(only submit) to v3
- Update Workflows to v3
- Rename Email to EmailSubscriptions
- Update many resources (Method's Visibility, Type Hinting etc)
- Repair majority of tests
- SingleEmail => TransactionEmail

## [1.0.0-rc.1]

### Added
- [CHANGELOG](http://keepachangelog.com/) @ryanwinchester
- Two new Exception classes @ryanwinchester

### Changed
- Namespace renamed from `Fungku\HubSpot` to `SevenShores\Hubspot` @ryanwinchester
- `Api` folder and namespace renamed to `Resources` @ryanwinchester
- The factory `HubSpotService` renamed to `Factory` @ryanwinchester
- The named static constructors in `Factory` were changed to `create()` and `createWithToken()` @ryanwinchester
- The `Factory` constructor was also made public @ryanwinchester
- Moved functionality of `Api` into `Client` and replaced `Api` with `Resource` @ryanwinchester
- `Client` is now constructed with a configuration array @ryanwinchester
- Removed `$base_url` in favour of putting the whole endpoint url in the resource methods. @ryanwinchester
- Optional `HUBSPOT_API_KEY` environment variable changed to `HUBSPOT_SECRET` @ryanwinchester
- Made `$data` property of `Response` public. Because why not? @ryanwinchester

### Fixed
- Trying to return a response with`RequestException` in the `Client`. It now re-throws a new `BadRequest` Exception. [#48](https://github.com/ryanwinchester/hubspot-php/issues/48) @ryanwinchester

[Unreleased]: https://github.com/ryanwinchester/hubspot-php/compare/v1.0.0-rc.1...HEAD
[1.0.0-rc.1]: https://github.com/ryanwinchester/hubspot-php/compare/v0.9.11...v1.0.0-rc.1
