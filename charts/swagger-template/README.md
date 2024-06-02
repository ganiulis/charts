# Swagger Deployment Template

### Instructions

1. Add this repository to Helm: `helm repo add swagger-deployment-template https://ganiulis.github.io/swagger-deployment-template`.
2. Create a default `values.yaml` from the chart: `helm show values swagger-deployment-template/swagger-deployment-template > values.yaml`.
3. Tweak `values.yaml` according to your needs.
4. Create an `swagger.json` inside `charts` and adjust it to your needs. It is used by Swagger UI.
5. Deploy this chart with `helm install [RELEASE_NAME] swagger-deployment-template/swagger-deployment-template -f values.yaml`.
6. _Optional:_ uninstall the chart with `helm uninstall [RELEASE_NAME]`.he chart with `helm uninstall [RELEASE_NAME]`.
