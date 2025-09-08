<!-- Warning: Do not manually edit this file. See notes on gluon + helm-docs at the end of this file for more information. -->
# prometheus-operator-crds

![Version: 23.0.0-bb.0](https://img.shields.io/badge/Version-23.0.0--bb.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.85.0](https://img.shields.io/badge/AppVersion-v0.85.0-informational?style=flat-square) ![Maintenance Track: bb_sandbox](https://img.shields.io/badge/Maintenance_Track-bb_sandbox-red?style=flat-square)

A Helm chart that collects custom resource definitions (CRDs) from the Prometheus Operator, allowing for seamless
integration with GitOps tools

## Upstream References

- <https://github.com/prometheus-community/helm-charts>

## Upstream Release Notes

This package has no upstream release note links on file. Please add some to [chart/Chart.yaml](chart/Chart.yaml) under `annotations.bigbang.dev/upstreamReleaseNotesMarkdown`.
Example:
```yaml
annotations:
  bigbang.dev/upstreamReleaseNotesMarkdown: |
    - [Find our upstream chart's CHANGELOG here](https://link-goes-here/CHANGELOG.md)
    - [and our upstream application release notes here](https://another-link-here/RELEASE_NOTES.md)
```

## Learn More

- [Application Overview](docs/overview.md)
- [Other Documentation](docs/)

## Pre-Requisites

- Kubernetes Cluster deployed
- Kubernetes config installed in `~/.kube/config`
- Helm installed

Kubernetes: `>=1.16.0-0`

Install Helm

https://helm.sh/docs/intro/install/

## Deployment

- Clone down the repository
- cd into directory

```bash
helm install prometheus-operator-crds chart/
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| upstream.crds.annotations | object | `{}` |  |
| upstream.crds.alertmanagerconfigs.enabled | bool | `true` |  |
| upstream.crds.alertmanagers.enabled | bool | `true` |  |
| upstream.crds.podmonitors.enabled | bool | `true` |  |
| upstream.crds.probes.enabled | bool | `true` |  |
| upstream.crds.prometheusagents.enabled | bool | `true` |  |
| upstream.crds.prometheuses.enabled | bool | `true` |  |
| upstream.crds.prometheusrules.enabled | bool | `true` |  |
| upstream.crds.scrapeconfigs.enabled | bool | `true` |  |
| upstream.crds.servicemonitors.enabled | bool | `true` |  |
| upstream.crds.thanosrulers.enabled | bool | `true` |  |

## Contributing

Please see the [contributing guide](./CONTRIBUTING.md) if you are interested in contributing.

---

_This file is programatically generated using `helm-docs` and some BigBang-specific templates. The `gluon` repository has [instructions for regenerating package READMEs](https://repo1.dso.mil/big-bang/product/packages/gluon/-/blob/master/docs/bb-package-readme.md)._

