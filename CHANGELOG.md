# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.8.2] - 2024-02-12

### Changed

- Adapt templates to be able to enable/disable apps.
- Add dependencies on `prometheus-operator-crd` for quicker deployment
- Update observability-bundle to v1.2.1
- Added values for security-bundle to re-enable PSPs

## [0.8.1] - 2024-01-17

### Fixed

- Fix psp values for observability-bundle > 1.0.0.

## [0.8.0] - 2024-01-15

### Changed

- Bump observability-bundle to 1.0.0. Beware that this version contains breaking changes

## [0.7.0] - 2023-12-13

### Added

- Add `security-bundle` app.

## [0.6.0] - 2023-12-11

### Added

- Add `teleport-kube-agent-app`

## [0.5.0] - 2023-11-27

### Fixed

- Shortened `etcd-kubernetes-resources-count-exporter` appName to `etcd-k8s-res-count-exporter`.

## [0.4.0] - 2023-11-20

## [0.3.0] - 2023-10-09

### Added

- Added `chart-operator-extension` version `v1.1.1` that contains e.g. `ServiceMonitors` for `chart-operator`.

## [0.2.0] - 2023-10-02

### Changed

- Upgrade `cert-manager-app` to [v3.4.0](https://github.com/giantswarm/cert-manager-app/releases/tag/v3.4.0)

## [0.1.0] - 2023-08-31

### Changed

- Set `external-dns` config for upgrade to v3.
- Set `chart-operator.giantswarm.io/force-helm-upgrade` annotation to `false` for `cert-manager` App CR.
- Enable cilium NetworkPolicies for `cert-manager`.

## [0.0.24] - 2023-08-03

### Changed

- :boom: Migrate CNI / CPI / CSI and VPA CRD apps to helmreleases to cluster-azure - requires `cluster-azure-app` 0.0.29

## [0.0.23] - 2023-07-31

### Added

- Add `etcd-kubernetes-resources-count-exporter`.
- Update `cert-manager-app` values in preparation of v3.0.0 release.

### Changed

- Change etcd prefix for `etcd-kubernetes-resources-count-exporter`.

## [0.0.22] - 2023-06-06

### Changed

- Add `cert-manager` app to default-apps-azure with version `2.21.0`
- Bump `cilium-app` to 0.10.0 - Renovate

## [0.0.21] - 2023-06-01

### Changed

- :boom: Remove workaround for VPA Seccomp
  - requires PSP from `cluster-shared v0.6.5` which ships with `cluster-azure 0.0.23`
- Bump `cert-exporter` to 2.6.0
- Bump `net-exporter` to 1.16.0
- Bump `observability-bundle` to 0.6.0 - Renovate
- Bump `core-dns-app` to 1.17.0 - Renovatge

## [0.0.20] - 2023-05-31

### Changed

- Bump `azure-cloud-controller-manager` to 1.24.18-gs4
  - Remove custom nodeSelector

## [0.0.19] - 2023-05-18

### Changed

- :boom: Disable `Seccomp` for VPA since is preventing pods from starting
  - This will be reverted once the problem is fixed

## [0.0.18] - 2023-05-17

### Changed

- Bump `azure-cloud-controller-manager` to 1.24.18-gs3
- Bump `azure-cloud-node-manager` to 1.24.18-gs3
- Bump `observability-bundle` to 0.5.1
- Bump `azuredisk-csi-driver` to 1.26.2-gs3
- Bump `external-dns` to 2.37.0

## [0.0.17] - 2023-05-15

### Changed

- Bump `observability-bundle` to 0.4.2
- :boom: Breaking - Update `Cilium Values` to enable `kube-proxy-replacement`
  - This change also require `cluster-azure` app >= 0.0.21
- Bump `cilium-app` to 0.9.3
- Bump `vertical-pod-autoscaler` to 3.4.2
- Bump `node-exporter` to 1.16.0
- Bump `net-exporter` to 1.15.0
- Bump `metrics-server` to 2.2.0
- Bump `cert-exporter` to 2.5.1
- Bump `azuredisk-csi-driver` to 1.26.2-gs2
- Bump `coredns-app` to 1.16.0
  - Remove custom nodeSelector for coredns since is no longer required

## [0.0.16] - 2023-04-18

### Changed

- Update `vertical-pod-autoscaler-app` to 3.4.1 to address PDB on single replicas pods issue

### Removed

- Remove kube-state-metrics app as it is now included in the observability-bundle.

## [0.0.15] - 2023-04-05

### Changed

- :boom: Reverting the `cilium kube-proxy replacement` feature because it is breaking NMI

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

[Unreleased]: https://github.com/giantswarm/default-apps-azure/compare/v0.8.2...HEAD
[0.8.2]: https://github.com/giantswarm/default-apps-azure/compare/v0.8.1...v0.8.2
[0.8.1]: https://github.com/giantswarm/default-apps-azure/compare/v0.8.0...v0.8.1
[0.8.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.7.0...v0.8.0
[0.7.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.6.0...v0.7.0
[0.6.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.5.0...v0.6.0
[0.5.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.24...v0.1.0
[0.0.24]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.23...v0.0.24
[0.0.23]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.22...v0.0.23
[0.0.22]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.21...v0.0.22
[0.0.21]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.20...v0.0.21
[0.0.20]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.19...v0.0.20
[0.0.19]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.18...v0.0.19
[0.0.18]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.17...v0.0.18
[0.0.17]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.16...v0.0.17
[0.0.16]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.15...v0.0.16
[0.0.15]: https://github.com/giantswarm/default-apps-azure/compare/v0.0.14...v0.0.15
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
