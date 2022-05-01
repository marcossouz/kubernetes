kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.0/aio/deploy/recommended.yaml
kubectl proxy
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/

kubectl apply -f service-account.yml
kubectl apply -f role-bidding.yml
kubectl -n kubernetes-dashboard get secret $(kubectl -n kubernetes-dashboard get sa/minikube -o jsonpath="{.secrets[0].name}") -o go-template="{{.data.token | base64decode}}"

token
eyJhbGciOiJSUzI1NiIsImtpZCI6ImZPeXpNZ21hd2NKZlk4dmZsak9pRFRFV2FRQkpLVHVURUg3X3VBYWktOEEifQ.eyJpc3MiOiJrdWJlcm5ldGVzL3NlcnZpY2VhY2NvdW50Iiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9uYW1lc3BhY2UiOiJrdWJlcm5ldGVzLWRhc2hib2FyZCIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VjcmV0Lm5hbWUiOiJtaW5pa3ViZS10b2tlbi0yc2Q4MiIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VydmljZS1hY2NvdW50Lm5hbWUiOiJtaW5pa3ViZSIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VydmljZS1hY2NvdW50LnVpZCI6ImIyZTQ5M2M3LWE0NzQtNDFhZS04OGE3LWNhOTAwYjE1Mjc0NCIsInN1YiI6InN5c3RlbTpzZXJ2aWNlYWNjb3VudDprdWJlcm5ldGVzLWRhc2hib2FyZDptaW5pa3ViZSJ9.L3izKWxbuTnAKsUhC-Vs6ET-HBylSdgW5NBetZZf8uLDNkEiNhM8CVHHk0wYvMIVygrZkj4oxXhG8SThoTQ35Vv2lNOri61LA3r66kFcYyZX-itfKXH3MT3hRFXsP7xaWoziabA2zPuOkQrfMkYg2o78sklQLBqCg8Xn1M-81Y7Hym0EbGTv0S-D2XIGRzDPF6yzPisRYM3GpuHdZCxQByxOVXqeenxJKKIUXLCCtK2Wk5PJVfRfEfqNQB_gGC-LnOcWoVCCEpwkhp-VjJwqrh98GBg9ahdnO9NkO684Drm0cEiMspnb4ZBOdKul5D0Gw0dLZCetKjUtvotQp6EnFQ

https://github.com/kubernetes-sigs/metrics-server
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml

--watch


$ curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
$ chmod 700 get_helm.sh
$ ./get_helm.sh

git clone https://github.com/benc-uk/kubeview
cd kubeview/charts/
helm install kubeview kubeview

kubectl get --namespace default svc -w kubeview