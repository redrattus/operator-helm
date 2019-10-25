# operator-helm

Operator-helm is the operator colletions for OpenStack.
Each chart deploys an operator and its CRDs.
For example, you can install prometheus operator and prometheus server, exporters using only one chart `prometheus-operator`.

You can use below extended operator charts.

| Operator Name | Features |
|---------------|----------|
| Prometheus Operator | * Support new exporters (openstack, process, bird...) <br/> * Deploy Push-gateway |
| Rook | * Make general rook chart to support multi storage type <br/> * Configure Cluster, BlockDevice, ObjectStorage, so on |
| Elasticsearch cloud k8s | * Deploy kibana <br/> * Configure Elasticsearch |

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


