# Pulse Helm charts

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```bash
#helm repo add pulse https://rcourtman.github.io/pulse/
helm repo add pulse https://ampls.github.io/Pulse/
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
pulse` to see the charts.

To install the `pulse` chart:

```bash
helm install my-pulse pulse/pulse
```

To install a specific pulse helm chart version in a specific namespace:

```bash
helm install my-pulse pulse/pulse -n awx --create-namespace -f my-values.yml --version 4.27.1
```

To uninstall the chart:

```bash
helm delete my-pulse
```
