# Values schema documentation

This page lists all available configuration options, based on the [configuration values schema](values.schema.json).

<!-- DOCS_START -->

### Apps

Properties within the `.apps` top-level object

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `apps.certExporter` |**None**|**Type:** `object`<br/>|
| `apps.certExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.certExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.certManager` |**None**|**Type:** `object`<br/>|
| `apps.certManager.appName` |**None**|**Type:** `string`<br/>|
| `apps.certManager.catalog` |**None**|**Type:** `string`<br/>|
| `apps.certManager.chartName` |**None**|**Type:** `string`<br/>|
| `apps.certManager.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.certManager.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.certManager.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.certManager.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.certManager.namespace` |**None**|**Type:** `string`<br/>|
| `apps.certManager.version` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions` |**None**|**Type:** `object`<br/>|
| `apps.chartOperatorExtensions.appName` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.catalog` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.chartName` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.chartOperatorExtensions.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.enabled` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.namespace` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.version` |**None**|**Type:** `string`<br/>|
| `apps.etcdKubernetesResourceCountExporter` |**None**|**Type:** `object`<br/>|
| `apps.etcdKubernetesResourceCountExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.etcdKubernetesResourceCountExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.etcdKubernetesResourceCountExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.etcdKubernetesResourceCountExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.etcdKubernetesResourceCountExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.etcdKubernetesResourceCountExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.etcdKubernetesResourceCountExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.etcdKubernetesResourceCountExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.etcdKubernetesResourceCountExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.external-dns` |**None**|**Type:** `object`<br/>|
| `apps.external-dns.appName` |**None**|**Type:** `string`<br/>|
| `apps.external-dns.catalog` |**None**|**Type:** `string`<br/>|
| `apps.external-dns.chartName` |**None**|**Type:** `string`<br/>|
| `apps.external-dns.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.external-dns.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.external-dns.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.external-dns.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.external-dns.namespace` |**None**|**Type:** `string`<br/>|
| `apps.external-dns.version` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer` |**None**|**Type:** `object`<br/>|
| `apps.metricsServer.appName` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.catalog` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.chartName` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.metricsServer.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.namespace` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.version` |**None**|**Type:** `string`<br/>|
| `apps.netExporter` |**None**|**Type:** `object`<br/>|
| `apps.netExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.netExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter` |**None**|**Type:** `object`<br/>|
| `apps.nodeExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.nodeExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle` |**None**|**Type:** `object`<br/>|
| `apps.observabilityBundle.appName` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.catalog` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.chartName` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.observabilityBundle.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.namespace` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.version` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent` |**None**|**Type:** `object`<br/>|
| `apps.teleport-kube-agent.appName` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent.catalog` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent.chartName` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.teleport-kube-agent.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.teleport-kube-agent.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.teleport-kube-agent.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.teleport-kube-agent.extraConfigs[*]` |**None**||
| `apps.teleport-kube-agent.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.teleport-kube-agent.namespace` |**None**|**Type:** `string`<br/>|
| `apps.teleport-kube-agent.version` |**None**|**Type:** `string`<br/>|
| `apps.vpa` |**None**|**Type:** `object`<br/>|
| `apps.vpa.appName` |**None**|**Type:** `string`<br/>|
| `apps.vpa.catalog` |**None**|**Type:** `string`<br/>|
| `apps.vpa.chartName` |**None**|**Type:** `string`<br/>|
| `apps.vpa.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.vpa.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.vpa.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.vpa.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.vpa.namespace` |**None**|**Type:** `string`<br/>|
| `apps.vpa.version` |**None**|**Type:** `string`<br/>|

### User Config

Properties within the `.userConfig` top-level object

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `userConfig.certManager` |**None**|**Type:** `object`<br/>|
| `userConfig.certManager.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.certManager.configMap.values` |**None**|**Type:** `string`<br/>|
| `userConfig.etcdKubernetesResourceCountExporter` |**None**|**Type:** `object`<br/>|
| `userConfig.etcdKubernetesResourceCountExporter.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.etcdKubernetesResourceCountExporter.configMap.values` |**None**|**Type:** `string`<br/>|
| `userConfig.external-dns` |**None**|**Type:** `object`<br/>|
| `userConfig.external-dns.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.external-dns.configMap.values` |**None**|**Type:** `string`<br/>|

### Other

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `clusterName` |**None**|**Type:** `string`<br/>|
| `organization` |**None**|**Type:** `string`<br/>|

<!-- DOCS_END -->
