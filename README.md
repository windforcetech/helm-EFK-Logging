## Elasticsearch, Fluentd, and Kibana
helm charts to create EFK (Elasticsearch, Fluentd, and Kibana) stack in kubernetes.

## Installation

step 1:
clone the repository:
```
git clone https://github.com/prameswar/efk-helm.git
```

step 2:
Install helm charts:
```
cd efk-helm
helm install fluentd
helm install elasticsearch
helm install kibana

```
To setup EFK Stack from single YAML File  elastic-fluentd-kibana.yaml
kubectl create -f elastic-fluentd-kibana.yaml




