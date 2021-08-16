# transmission

![Version: 6.6.0](https://img.shields.io/badge/Version-6.6.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: auto](https://img.shields.io/badge/AppVersion-auto-informational?style=flat-square)

API Support for your favorite torrent trackers.

**Homepage:** <https://github.com/truecharts/apps/tree/master/charts/stable/transmission>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| TrueCharts | info@truecharts.org | truecharts.org |
| Ornias1993 | kjeld@schouten-lebbing.nl | truecharts.org |

## Source Code

* <https://github.com/transmission/transmission>
* <https://hub.docker.com/r/linuxserver/transmission>

## Requirements

Kubernetes: `>=1.16.0-0`

| Repository | Name | Version |
|------------|------|---------|
| https://truecharts.org/ | common | 6.8.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| env | object | `{}` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/k8s-at-home/transmission"` |  |
| image.tag | string | `"v3.00"` |  |
| persistence.config.enabled | bool | `true` |  |
| persistence.config.mountPath | string | `"/config"` |  |
| persistence.config.type | string | `"emptyDir"` |  |
| service.main.ports.main.port | int | `9091` |  |
| service.torrent.enabled | bool | `true` |  |
| service.torrent.ports.tcp.enabled | bool | `true` |  |
| service.torrent.ports.tcp.port | int | `51413` |  |
| service.torrent.ports.tcp.protocol | string | `"TCP"` |  |
| service.torrent.ports.udp.enabled | bool | `true` |  |
| service.torrent.ports.udp.port | int | `51413` |  |
| service.torrent.ports.udp.protocol | string | `"UDP"` |  |
| service.torrent.type | string | `"ClusterIP"` |  |
| strategy.type | string | `"Recreate"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)