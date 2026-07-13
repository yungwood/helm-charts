# helm-charts

Public Helm chart repository for charts maintained by [yungwood](https://github.com/yungwood).

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up, add the repo:

```console
helm repo add yungwood https://yungwood.github.io/helm-charts/
```

You can then run `helm search repo yungwood` to see the charts.

## Charts

- [ical-filter-proxy](https://github.com/yungwood/helm-charts/tree/master/charts/ical-filter-proxy)
  - Application: [yungwood/ical-filter-proxy](https://github.com/yungwood/ical-filter-proxy)
  - Source of truth: synced from the application repository

```bash
helm install your-release yungwood/ical-filter-proxy
```

Also see [artifact hub](https://artifacthub.io/packages/search?repo=yungwood) for a complete list.

## Publishing

Chart releases are published from this repository to GitHub Pages at:

```text
https://yungwood.github.io/helm-charts/
```

Changes under `charts/` are linted and install-tested on pull requests. Merged
chart changes on the default branch are packaged and released by GitHub Actions.

For application charts, the preferred workflow is for the application repository
to own the chart source alongside the application code, then sync the rendered
chart directory into this repository under `charts/<chart-name>`. This keeps the
chart close to the app it deploys while preserving a single public Helm
repository URL.

For standalone charts, the chart source may live directly in this repository.
