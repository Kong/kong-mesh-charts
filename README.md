![Kong Mesh](./artifacts/kong-mesh.png)

# Kong Mesh Helm Charts

## Add the Kong Mesh Helm repository

```sh
helm repo add kong-mesh https://kong.github.io/kong-mesh-charts
```

## Install Kong Mesh with Helm

```sh
helm upgrade -i kong-mesh kong-mesh/kong-mesh
```
## Source Code

The charts are published in this repo's [gh-pages branch](https://github.com/kong/kong-mesh-charts/tree/gh-pages)

Artifact Hub references to these charts at https://artifacthub.io/packages/helm/kong-mesh/kong-mesh

### License

[Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0)
