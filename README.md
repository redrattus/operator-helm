# operator-helm

Operator-helm is the operator colletions for OpenStack.
Each chart deploys an operator and its CRDs.
For example, you can install prometheus operator and prometheus server, exporters using only one chart `prometheus-operator`.

## How to use
```
git clone https://github.com/openinfradev/operator-helm
cd operator-helm

# install prometheus
helm install --name prometheus prometheus-operator/

# install rook
helm install --name rook rook/

# install eck
helm install --name eck elasticsearch-cloud-k8s/
```


