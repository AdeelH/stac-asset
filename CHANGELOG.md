# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.2] - 2023-09-18

### Added

- `read_href` and `blocking.read_href` ([#107](https://github.com/stac-utils/stac-asset/pull/107))

## [0.2.1] - 2023-09-05

### Fixed

- Use absolute paths for item collection downloads ([#96](https://github.com/stac-utils/stac-asset/pull/96), [#97](https://github.com/stac-utils/stac-asset/pull/97))

## [0.2.0] - 2023-08-23

### Added

- Use multiple clients when downloading ([#46](https://github.com/stac-utils/stac-asset/pull/46))
- `--alternate-assets` option to the CLI ([#46](https://github.com/stac-utils/stac-asset/pull/46))
- Content-type checking ([#46](https://github.com/stac-utils/stac-asset/pull/46), [#60](https://github.com/stac-utils/stac-asset/issues/60))
- `Client.from_config` and `Client.close` ([#46](https://github.com/stac-utils/stac-asset/pull/46))
- Retry configuration for S3 ([#47](https://github.com/stac-utils/stac-asset/pull/47))
- `Collection` download ([#50](https://github.com/stac-utils/stac-asset/pull/50))
- Progress reporting ([#55](https://github.com/stac-utils/stac-asset/pull/55), [#69](https://github.com/stac-utils/stac-asset/pull/69))
- `ErrorStrategy` ([#69](https://github.com/stac-utils/stac-asset/pull/69))
- `fail_fast` ([#69](https://github.com/stac-utils/stac-asset/pull/69))
- `assert_asset_exists`, `asset_exists`, `Client.assert_href_exists`, `Client.href_exists` ([#81](https://github.com/stac-utils/stac-asset/pull/81), [#85](https://github.com/stac-utils/stac-asset/pull/85))
- Blocking interface ([#86](https://github.com/stac-utils/stac-asset/pull/86))
- `stac-asset info` CLI subcommand ([#82](https://github.com/stac-utils/stac-asset/pull/83))

### Changed

- Use `Config` instead of standalone arguments ([#45](https://github.com/stac-utils/stac-asset/pull/45), [#67](https://github.com/stac-utils/stac-asset/pull/67))
- Re-use the same client for an entire item collection ([#59](https://github.com/stac-utils/stac-asset/pull/59))
- If `include` or `exclude` is used, the un-included assets are removed from the source object ([#70](https://github.com/stac-utils/stac-asset/pull/70))

### Removed

- USGS EROS client ([#37](https://github.com/stac-utils/stac-asset/pull/37))
- `Client.default` ([#46](https://github.com/stac-utils/stac-asset/pull/46))
- `Client.download_asset` ([#68](https://github.com/stac-utils/stac-asset/pull/68))

## [0.1.1] - 2023-07-12

### Fixed

- Add `py.typed` ([#35](https://github.com/stac-utils/stac-asset/pull/35))

## [0.1.0] - 2023-07-12

First release at the new location, <https://github.com/stac-utils/stac-asset>.
Used to be <https://github.com/gadomski/stac-asset>.

## [0.0.4] - 2023-06-09

### Added

- `Client.download_item_collection()` ([#20](https://github.com/stac-utils/stac-asset/pull/20))
- Command-line interface ([#22](https://github.com/stac-utils/stac-asset/pull/22), [#23](https://github.com/stac-utils/stac-asset/pull/23))

### Changed

- Behavior of the item file name in `Client.download_item()` ([#20](https://github.com/stac-utils/stac-asset/pull/20))

## [0.0.3] - 2023-05-31

### Added

- Warnings instead of errors if assets are missing
- Ability to save assets with their key as their file name
- Earthdata client

### Changed

- `download_item` returns the modified item

### Fixed

- All relative hrefs are made absolute on item download
- Clean up local files on download error

### Removed

- `open_asset` and `download_asset`

## [0.0.2] - 2023-05-25

### Added

- `stac_asset.download_item_from_href`
- Requester-pays support to the s3 client

### Fixed

- Cleaning up connections is easier thanks to `__aexit__` implementations

## [0.0.1] - 2023-05-24

Initial release.

[unreleased]: https://github.com/stac-utils/stac-asset/compare/v0.2.2...HEAD
[0.2.2]: https://github.com/stac-utils/stac-asset/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/stac-utils/stac-asset/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/stac-utils/stac-asset/compare/v0.1.1...v0.2.0
[0.1.1]: https://github.com/stac-utils/stac-asset/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/stac-utils/stac-asset/compare/v0.0.4...v0.1.0
[0.0.4]: https://github.com/stac-utils/stac-asset/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/stac-utils/stac-asset/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/stac-utils/stac-asset/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/stac-utils/stac-asset/releases/tag/v0.0.1
