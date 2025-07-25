# redis

![Version: 0.8.2](https://img.shields.io/badge/Version-0.8.2-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 6.2.14-alpine](https://img.shields.io/badge/AppVersion-6.2.14--alpine-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| global.imagePullSecrets | list | `[]` |  |
| global.storageClass | string | `""` |  |
| imagePullSecrets | object | `{}` |  |
| initContainers.config_init.image.digest | string | `""` |  |
| initContainers.config_init.image.pullPolicy | string | `"IfNotPresent"` |  |
| initContainers.config_init.image.pullSecrets | list | `[]` |  |
| initContainers.config_init.image.registry | string | `"docker.io"` |  |
| initContainers.config_init.image.repository | string | `"redis"` |  |
| initContainers.config_init.image.tag | string | `"6.2.14-alpine"` |  |
| metrics.enabled | bool | `false` |  |
| metrics.image.digest | string | `""` |  |
| metrics.image.pullPolicy | string | `"IfNotPresent"` |  |
| metrics.image.registry | string | `"docker.io"` |  |
| metrics.image.repository | string | `"oliver006/redis_exporter"` |  |
| metrics.image.tag | string | `"latest"` |  |
| metrics.resources | object | `{}` |  |
| metrics.serviceMonitor.enabled | bool | `false` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.fsGroup | int | `1000` |  |
| podSecurityContext.runAsNonRoot | bool | `true` |  |
| podSecurityContext.runAsUser | int | `1000` |  |
| redis.image.digest | string | `""` |  |
| redis.image.pullPolicy | string | `"IfNotPresent"` |  |
| redis.image.pullSecrets | list | `[]` |  |
| redis.image.registry | string | `"docker.io"` |  |
| redis.image.repository | string | `"redis"` |  |
| redis.image.tag | string | `"6.2.14-alpine"` |  |
| redis.resources.limits.memory | string | `"200Mi"` |  |
| redis.resources.requests.cpu | float | `0.1` |  |
| redis.resources.requests.memory | string | `"200Mi"` |  |
| replicaCount | int | `3` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `65534` |  |
| sentinel.image.digest | string | `""` |  |
| sentinel.image.pullPolicy | string | `"IfNotPresent"` |  |
| sentinel.image.pullSecrets | list | `[]` |  |
| sentinel.image.registry | string | `"docker.io"` |  |
| sentinel.image.repository | string | `"redis"` |  |
| sentinel.image.tag | string | `"6.2.14-alpine"` |  |
| sentinel.resources.limits.memory | string | `"200Mi"` |  |
| sentinel.resources.requests.cpu | string | `"100m"` |  |
| sentinel.resources.requests.memory | string | `"200Mi"` |  |
| service.metricsPort | int | `9121` |  |
| service.sentinelport | int | `26379` |  |
| service.serverport | int | `6379` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| tolerations | list | `[]` |  |
| useAntiAffinity | bool | `true` | Enable Hard pod anti-affinity during scheduling |
| volumeClaimTemplate.resources.requests.storage | string | `"10Gi"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
