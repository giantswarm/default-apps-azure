# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Add Azure Cloud node manager.
- Add Azure `CSI` driver and overwrite default configuration for `CAPZ` based clusters.
- Add `CoreDNS`.
- Add icon url to `Chart.yaml`.
- Add `values.yaml` json schema.

### Changed

- Adopt `labels` to align with other default-apps.
- Prepare `cilium` default configuration for `CAPZ` based clusters.
- Bump Azure `CPI` to latest version and overwrite default configuration for `CAPZ` based clusters.

## [0.0.2] - 2022-11-30

### Changed

- Push to `cluster-catalog` and `cluster-test-catalog`

## [0.0.1] - 2022-11-22

### Added

- add `cilium` and Azure `CPI`

### Changed

- changed `app.giantswarm.io` label group was changed to `application.giantswarm.io`

[Unreleased]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.2...HEAD
[0.0.2]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/default-apps-azure/releases/tag/v0.0.1
