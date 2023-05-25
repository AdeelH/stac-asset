# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- `stac_asset.download_item_from_href`
- Requester-pays support to the s3 client

### Fixed

- Cleaning up connections is easier thanks to `__aexit__` implementations.

## [0.0.1] - 2023-05-24

Initial release.

[unreleased]: https://github.com/gadomski/stac-asset/compare/v0.0.1...HEAD
[0.0.1]: https://github.com/gadomski/stac-asset/releases/tag/v0.0.1
