# open-webui

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square)

Open WebUI: A User-Friendly Web Interface for Chat Interactions 👋

**Homepage:** <https://www.openwebui.com/>

## Source Code

* <https://github.com/open-webui/helm-charts>
* <https://github.com/open-webui/open-webui/pkgs/container/open-webui>
* <https://github.com/otwld/ollama-helm/>
* <https://hub.docker.com/r/ollama/ollama>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://helm.openwebui.com | pipelines | >=0.0.1 |
| https://otwld.github.io/ollama-helm/ | ollama | >=0.24.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"ghcr.io/open-webui/open-webui"` |  |
| image.tag | string | `"main"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"open-webui.example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.tls | list | `[]` |  |
| livenessProbe.httpGet.path | string | `"/"` |  |
| livenessProbe.httpGet.port | string | `"http"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| openWebui.data.accessModes[0] | string | `"ReadWriteOnce"` |  |
| openWebui.data.size | string | `"10Gi"` |  |
| openWebui.data.storageClassName | string | `""` |  |
| openWebui.env.DEFAULT_LOCALE | string | `"en_US.utf8"` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| readinessProbe.httpGet.path | string | `"/"` |  |
| readinessProbe.httpGet.port | string | `"http"` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| restartPolicy | string | `"Always"` |  |
| securityContext | object | `{}` |  |
| service.port | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| volumeMounts | list | `[]` |  |
| volumes | list | `[]` |  |

