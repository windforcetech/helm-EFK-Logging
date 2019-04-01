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


Monitoring Set-up using helm charts


helm install grafana
```
NOTES:
1. Get your 'admin' user password by running:

   kubectl get secret --namespace default unhinged-hare-grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo

2. The Grafana server can be accessed via port 80 on the following DNS name from within your cluster:

   unhinged-hare-grafana.default.svc.cluster.local

   Get the Grafana URL to visit by running these commands in the same shell:

     export POD_NAME=$(kubectl get pods --namespace default -l "app=grafana,release=unhinged-hare" -o jsonpath="{.items[0].metadata.name}")
     kubectl --namespace default port-forward $POD_NAME 3000
 ```
helm install prometheus

```
NOTES:
The Prometheus server can be accessed via port 80 on the following DNS name from within your cluster:
nomadic-heron-prometheus-server.default.svc.cluster.local


Get the Prometheus server URL by running these commands in the same shell:
  export POD_NAME=$(kubectl get pods --namespace default -l "app=prometheus,component=server" -o jsonpath="{.items[0].metadata.name}")
  kubectl --namespace default port-forward $POD_NAME 9090
```

helm install metric-server

