![Kong Mesh](./artifacts/kong-mesh.png)

# Kong Mesh Helm Charts

[![Artifact HUB](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/kong-mesh)](https://artifacthub.io/packages/search?repo=kong-mesh)

## Add the Kong Mesh Helm repository

```sh
helm repo add kong-mesh https://kong.github.io/kong-mesh-charts
```

## Installing Kong Mesh using the Helm Charts

Create the `kong-mesh-system` namespace:
```sh
kubectl create namespace kong-mesh-system
```

Upload the license secret to the cluster:
```sh
kubectl create secret generic kong-mesh-license -n kong-mesh-system --from-file=/path/to/license.json
```

NOTE: The name of the file *should* be `license.json`, unless otherwise specified in `values.yaml`.

Deploy the Kong Mesh Helm Chart:
```sh
helm upgrade -i -n kong-mesh-system kong-mesh kong-mesh/kong-mesh
```

## Artifact Hub

Artifact Hub references to these charts at https://artifacthub.io/packages/helm/kong-mesh/kong-mesh

### License

[Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0)
