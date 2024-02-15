.PHONY: deploy-addons
deploy-addons:
    kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/prometheus.yaml
    kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/kiali.yaml
    kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/jaeger.yaml
    kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/grafana.yaml

.PHONY: dashboard
deploy-addons:
    istioctl dashboard kiali