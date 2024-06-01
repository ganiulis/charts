# Charts

## Instructions

### Installation

1. Add this repo with `helm repo add ganiulis https://ganiulis.github.io/charts`.
2. Browse available charts with `helm search repo ganiulis`.
3. Fetch a `values.yaml` example with `helm show values ganiulis/... > values.yaml`.
4. Some repos require a secret. Create one with `kubectl create secret generic [CONTAINER_NAME]-env --from-env-file=[ENV_FILE]`.
5. Deploy the chart with `helm install [RELEASE_NAME] ganiulis/... -f values.yaml`.
6. Optional: run the test suite with `helm test [RELEASE_NAME]`.
7. Optional: uninstall the chart with `helm uninstall [RELEASE_NAME]`.
