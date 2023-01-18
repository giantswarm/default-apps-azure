# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Add `kube-state-metrics`
- Add `metrics-server`
- Add `vertical-pod-autoscaler`

## [0.0.6] - 2022-12-28

### Changed

* Bump `coredns-app` to v1.13.0

## [0.0.5] - 2022-12-27

### Added

- Configuration for `coredns` app to update nodeSelector of masters instance

## [0.0.4] - 2022-12-22

### Changed

- Update `azuredisk CSI` driver to 1.25.2-gs1
- Run `coredns` from test catalog so we can have a working DNS on capz ( need to test it on all other environments first )

## [0.0.3] - 2022-12-21

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

[Unreleased]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.6...HEAD
[0.0.6]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.5...v0.0.6
[0.0.5]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.4...v0.0.5
[0.0.4]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/default-apps-azure/releases/tag/v0.0.1
