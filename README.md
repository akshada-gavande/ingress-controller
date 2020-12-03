# ingress-controller -Steps
Minikube start
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/provider/baremetal/deploy.yaml
kubectl get pods -n ingress-nginx -l app.kubernetes.io/name=ingress-nginx
kubectl create -f httpd-deployment.yaml
kubectl create -f myweb-ingress.yaml
kubectl get ingress name-based-virtualhost-ingress
kubectl describe ingress name-based-virtualhost-ingress

