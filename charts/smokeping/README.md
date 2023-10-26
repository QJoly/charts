# smokeping

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.8.2](https://img.shields.io/badge/AppVersion-2.8.2-informational?style=flat-square)

SmokePing is a latency logging and graphing and alerting system

**Homepage:** <https://oss.oetiker.ch/smokeping/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| QJOLY | <github@thoughtless.eu> | <https://une-tasse-de.cafe> |

## Source Code

* <https://github.com/oetiker/SmokePing>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://rubxkube.github.io/common-charts | common | v0.2.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| common.app.containerPort | int | `80` |  |
| common.app.servicePort | int | `80` |  |
| common.deployment.cpuLimit | string | `nil` |  |
| common.deployment.cpuRequest | string | `nil` |  |
| common.deployment.memoryLimit | string | `nil` |  |
| common.deployment.memoryRequest | string | `nil` |  |
| common.deployment.strategy.rollingUpdate.maxSurge | string | `"25%"` |  |
| common.deployment.strategy.rollingUpdate.maxUnavailable | string | `"25%"` |  |
| common.deployment.strategy.type | string | `"RollingUpdate"` |  |
| common.hpa.avgCpuUtilization | int | `50` |  |
| common.hpa.enabled | bool | `false` |  |
| common.hpa.maxReplicas | int | `2` |  |
| common.hpa.minReplicas | int | `1` |  |
| common.image.pullPolicy | string | `"Always"` |  |
| common.image.repository | string | `"linuxserver/smokeping"` |  |
| common.image.repositorySettings.isPrivate | bool | `false` |  |
| common.image.repositorySettings.secretName | string | `nil` |  |
| common.image.tag | string | `"2.8.2"` |  |
| common.ingress.certResolver | string | `"letsencrypt"` |  |
| common.ingress.enabled | bool | `false` |  |
| common.ingress.entrypoint | string | `"websecure"` |  |
| common.ingress.hostName | string | `"smokeping.thoughtless.eu"` |  |
| common.ingress.ingressClassName | string | `nil` |  |
| common.ingress.isIngressRoute | bool | `true` |  |
| common.ingress.tls.enabled | bool | `true` |  |
| common.ingress.tls.secretName | string | `""` |  |
| common.livenessProbe.failureThreshold | int | `1` |  |
| common.livenessProbe.httpGet.path | string | `"/"` |  |
| common.livenessProbe.httpGet.port | int | `80` |  |
| common.livenessProbe.initialDelaySeconds | int | `30` |  |
| common.livenessProbe.periodSeconds | int | `60` |  |
| common.livenessProbe.timeoutSeconds | int | `3` |  |
| common.livenessProbeEnabled | bool | `true` |  |
| common.persistence.enabled | bool | `true` |  |
| common.persistence.volumes[0].containerMount | string | `"/data/"` |  |
| common.persistence.volumes[0].name | string | `"data"` |  |
| common.persistence.volumes[0].pvcClaim | string | `""` |  |
| common.persistence.volumes[0].size | string | `"5Gi"` |  |
| common.persistence.volumes[0].storageClassName | string | `""` |  |
| common.persistence.volumes[1].containerMount | string | `"/config/"` |  |
| common.persistence.volumes[1].name | string | `"config"` |  |
| common.persistence.volumes[1].pvcClaim | string | `""` |  |
| common.persistence.volumes[1].size | string | `"1Gi"` |  |
| common.persistence.volumes[1].storageClassName | string | `""` |  |
| common.readinessProbe.failureThreshold | int | `2` |  |
| common.readinessProbe.httpGet.path | string | `"/"` |  |
| common.readinessProbe.httpGet.port | int | `80` |  |
| common.readinessProbe.initialDelaySeconds | int | `30` |  |
| common.readinessProbe.periodSeconds | int | `30` |  |
| common.readinessProbe.timeoutSeconds | int | `3` |  |
| common.readinessProbeEnabled | bool | `true` |  |
| common.startupProbe.failureThreshold | int | `20` |  |
| common.startupProbe.httpGet.path | string | `"/"` |  |
| common.startupProbe.httpGet.port | int | `80` |  |
| common.startupProbe.periodSeconds | int | `10` |  |
| common.startupProbe.timeoutSeconds | int | `1` |  |
| common.startupProbeEnabled | bool | `true` |  |
| common.tests.classicHttp.enabled | bool | `true` |  |
| common.tests.curlHostHeader.enabled | bool | `true` |  |
| common.tests.curlHostHeader.path | string | `"/"` |  |
| common.variables.nonSecret | object | `{}` |  |
| common.variables.secret | object | `{}` |  |
| define | int | `80` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)