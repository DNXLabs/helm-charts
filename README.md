# helm-charts

Kubernetes helm charts repository.

## Dependencies

- Helm

## Usage

```
helm repo add dnx https://charts.dnx.one
helm repo update
```

## Test the Helm chart repository

```bash
helm search repo dnx
```

## Install chart repository

Helm 2
```bash
helm install --values values.yaml --name example --namespace example-ns dnx
```

Helm 3
```bash
helm install --values values.yaml --namespace example-ns example dnx
```

## Lint charts

```
make lint
```

## Package charts

```
make package
```

## Index charts

```
make index
```

## Author

Managed by [DNX Solutions](https://github.com/DNXLabs).

## License

Apache 2 Licensed. See [LICENSE](https://github.com/DNXLabs/helm-charts/blob/master/LICENSE) for full details.