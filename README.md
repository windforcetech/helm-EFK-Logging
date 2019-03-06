## Elasticsearch, Fluentd, and Kibana
helm charts to create EFK (Elasticsearch, Fluentd, and Kibana) stack in kubernetes.

## Installation

Step 1:
clone the repository:
```
git git@github.com:dhiruLeo/helm-EFK-Logging.git

```
Step 2:
Install helm charts:
```
Step 3:
cd efk-helm
helm install fluentd
helm install elasticsearch
helm install kibana

```
## Elasticsearch, Fluentd, and Kibana

To setup EFK Stack from single YAML File  
i.e. elastic-fluentd-kibana.yaml

kubectl create -f elastic-fluentd-kibana.yaml

```

