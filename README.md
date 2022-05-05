# DoSAttackData
Data extracted from DoS attacks using Cilium


Exported Cilium flows live here.

Data that cilium collected during the attack is here. 
The data is now directly pushed into prometheus which is then parsed by grafana to show different stats regarding attacks

## Setup

- Installed minikube without cilium
- Installed cilium using helm
  - Follow https://docs.cilium.io/en/stable/gettingstarted/k8s-install-helm/
- Install hubble using helm
- Enable http obersvaiblity in Cilium for the pod
- Install grafana and prometheus
  - Follow https://docs.cilium.io/en/stable/gettingstarted/grafana/
- Update hubble's settings to send data to prometheus

## Raw data
- Just `hubble observe > file` to dump all flows into a file


