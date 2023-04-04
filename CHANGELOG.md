# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.0.14] - 2023-04-04

### Changed

- :boom: Breaking - Update `Cilium Values` to enable `kube-proxy-replacement` 
  - This change also require `cluster-azure` app >= 0.0.17

## [0.0.13] - 2023-03-22

### Changed

- Bumped `vpa` to 3.3.0 and `vpaCRD` to 2.0.0

### Added

- New app dependency mechanism (`app-operator.giantswarm.io/depends-on`) to the vertical-pod-autoscaler-app it is not installed until the corresponding CRD app is deployed.

## [0.0.12] - 2023-03-07

### Added

- Add `external-dns`

## [0.0.11] - 2023-02-15

### Changed

- Bumped `azuredisk-csi-driver` to 1.26.2-gs1

## [0.0.10] - 2023-02-02

### Added

- Add `cert-exporter`
- Add `net-exporter`
- Add `node-exporter`

## [0.0.9] - 2023-01-24

### Changed

- `azuredisk-csi-driver` - remove settings to force controller on control-plane nodes

## [0.0.8] - 2023-01-18

### Added

- Add `observability-bundle`

## [0.0.7] - 2023-01-18

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

[Unreleased]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.14...HEAD
[0.0.14]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.13...v0.0.14
[0.0.13]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.12...v0.0.13
[0.0.12]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.11...v0.0.12
[0.0.11]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.10...v0.0.11
[0.0.10]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.9...v0.0.10
[0.0.9]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.8...v0.0.9
[0.0.8]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.7...v0.0.8
[0.0.7]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.6...v0.0.7
[0.0.6]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.5...v0.0.6
[0.0.5]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.4...v0.0.5
[0.0.4]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/default-apps-azure/releases/tag/v0.0.1
