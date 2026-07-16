<p align="center">
  <a href="https://yungwood.github.io/helm-charts/">
    <img src="pages/helm-charts.svg" alt="Helm charts logo" width="144">
  </a>
</p>

# helm-charts

Public Helm chart repository for charts maintained by [yungwood](https://github.com/yungwood).
Visit <https://yungwood.github.io/helm-charts/> for a browsable package list.

## Usage

To add the repo and show available charts:

```console
helm repo add yungwood https://yungwood.github.io/helm-charts/
helm search repo yungwood
```

Also see [artifact hub](https://artifacthub.io/packages/search?repo=yungwood) for a complete list.

## Publishing

Chart releases are published from this repository to GitHub Pages at:

```text
https://yungwood.github.io/helm-charts/
```

That page lists the published packages in this repository.

Changes under `charts/` are linted and install-tested on pull requests. Merged
chart changes on the default branch are packaged and released by GitHub Actions.
Human-facing and metadata files published to GitHub Pages are maintained in
`pages/` and copied to the published `gh-pages` branch by the release workflow.
The browser homepage is served from `pages/index.html`, with the shared logo at
`pages/helm-charts.svg`.

For application charts, the preferred workflow is for the application repository
to own the chart source alongside the application code, then sync the rendered
chart directory into this repository under `charts/<chart-name>`. This keeps the
chart close to the app it deploys while preserving a single public Helm
repository URL.

For standalone charts, the chart source may live directly in this repository.
