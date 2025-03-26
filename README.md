# volweb-chart

## Install
```bash
git clone https://github.com/JakePeralta7/volweb-chart/
cd volweb-chart
kubectl create namespace volweb
helm install volweb ./volweb-chart \
  --set ingress.hosts[0].host=<your-domain.com> \
  --set backend.env.CORS_ALLOWED_ORIGINS=https://<your-domain.com>:3000 \
  --namespace=volweb
```
