# Helm Charts Repository

This repository serves as a centralized location for all the Helm charts I have created. These charts simplify deploying and managing applications on Kubernetes by providing reusable and configurable deployment templates.

## Adding the Repository

To use the Helm charts from this repository, you can add it to your Helm configuration with the following command:

```bash
helm repo add ammarlakis https://ammarlakis.github.io/helm-charts/
```

## Available Charts

Below is the list of Helm charts available in this repository:

- **[Home Assistant](https://github.com/ammarlakis/home-assistant-chart)**: A Helm chart for deploying Home Assistant on Kubernetes. It supports dynamic configuration, restores, and integrates with popular Kubernetes tools.

## Usage

To deploy a chart from this repository, use the following steps:

1. Search for the desired chart:
   ```bash
   helm search repo ammarlakis
   ```

2. Install the chart:
   ```bash
   helm install <release-name> ammarlakis/<chart-name> --namespace <namespace>
   ```

   Replace `<release-name>`, `<chart-name>`, and `<namespace>` with your preferred release name, the name of the chart, and the namespace where you want to deploy the application.

3. (Optional) Customize values by creating a `values.yaml` file and providing it during installation:
   ```bash
   helm install <release-name> ammarlakis/<chart-name> -f values.yaml --namespace <namespace>
   ```

## Contributing

If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on the respective chart's repository.

## License

This repository and the included Helm charts are open-source and distributed under the [MIT License](LICENSE).
