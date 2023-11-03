## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

    helm repo add my-repo https://yakir3.github.io/helm-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  
You can then run `helm search repo my-repo` to see the charts.

To install the my-app chart:

    helm install my-app my-repo/my-app

To uninstall the chart:

    helm delete my-app



To index helm repo

    # 1.package chart
    cd docs
    helm package ../charts/*
    # 2.generated helm index docs
    helm repo index ../docs --url https://359sun.top/helm-charts
    # 3.push to repo
    git push origin
