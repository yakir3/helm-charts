## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add yakir-helm-repo https://yakir3.github.io/helm-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
yakir-helm-repo` to see the charts.

To install the my-prometheus-app chart:

    helm install my-prometheus-app yakir-helm-repo/prometheus-app

To uninstall the chart:

    helm delete my-prometheus-app
