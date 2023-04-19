### vela安装.

```javascript
curl -fsSl https://kubevela.net/script/install.sh | bash
vela install
vela addon enable velaux serviceType=LoadBalancer
vela web登录：admin VelaUX12345
vela addon enable kube-state-metrics
vela addon enable node-exporter
vela addon enable prometheus-server thanos=true serviceType=LoadBalancer storage=5G
vela addon enable loki agent=vector serviceType=LoadBalancer storage=10G
vela addon enable grafana serviceType=LoadBalancer storage=10G
grafana web登录： admin kubevela
```
