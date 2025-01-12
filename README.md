# helm-charts

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repo as follows:

```console
helm repo add yungwood https://yungwood.github.io/helm-charts/
```

You can then run `helm search repo yungwood` to see the charts.

## Charts

- [ical-filter-proxy](https://github.com/yungwood/helm-charts/tree/master/charts/ical-filter-proxy)

```bash
helm install --name your-release yungwood/ical-filter-proxy
```

Also see [artifact hub](https://artifacthub.io/packages/search?repo=yungwood) for a complete list.
