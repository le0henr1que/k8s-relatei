.PHONY: deploy-addons
deploy-addons:
	kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/prometheus.yaml \
	&& kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/kiali.yaml \
	&& kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/jaeger.yaml \
	&& kubectl apply -f https://raw.githubusercontent.com/istio/istio/master/samples/addons/grafana.yaml

.PHONY: dashboard
dashboard:
	istioctl dashboard kiali

.PHONY: deploy-fortio
deploy-fortio:
	kubectl apply -f https://raw.githubusercontent.com/istio/istio/release-1.9/samples/httpbin/sample-client/fortio-deploy.yaml
