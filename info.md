kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.0/aio/deploy/recommended.yaml
kubectl proxy
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/

kubectl apply -f service-account.yml
kubectl apply -f role-bidding.yml
kubectl -n kubernetes-dashboard get secret $(kubectl -n kubernetes-dashboard get sa/minikube -o jsonpath="{.secrets[0].name}") -o go-template="{{.data.token | base64decode}}"


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
