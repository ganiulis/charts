# Charts

## Instructions

### Installation

1. Add this repo with `helm repo add ganiulis https://ganiulis.github.io/charts`.
2. Browse available charts with `helm search repo ganiulis`.
3. Fetch a `values.yaml` example with `helm show values ganiulis/... > values.yaml`.
4. Some repos require a Secret to hold environmental variables. Create one with `kubectl create secret generic [CONTAINER_NAME]-env --from-env-file=[ENV_FILE]`.
5. Deploy the chart with `helm install [RELEASE_NAME] ganiulis/... -f values.yaml`.
6. Optional: uninstall the chart with `helm uninstall [RELEASE_NAME]`.

### Notes

- The Swagger UI template requires a `swagger.json` file. Create a ConfigMap for it with `kubectl create configmap [RELEASE_NAME] --from-file=[SWAGGER_JSON_FILE]`. Once created restart the deployment with `kubectl rollout restart deployment/[RELEASE_NAME]`.
