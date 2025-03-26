# volweb-chart

## Install
```bash
kubectl create namespace volweb
helm install volweb ./volweb-chart \
  --set ingress.hosts[0].host=your-domain.com \
  --namespace=volweb
```
