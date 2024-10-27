# my notes to learn kubernetes with minikube


- This tutorial using minikube and kubectl please do install if you want to follow

## BASIC COMMAND
- kubectl get nodes | kubectl get nodes -o wide #to see running nodes
- kubectl get deployment | kubectl get deployment -o wide #to see running deployment
- kubectl get pods | kubectl get pods-o wide #to see running pods
- kubectl get services | kubectl get svc | kubectl get svc -o wide | # to see running services 
- kubectl get ingress | kubectl get ingress -o wide #to see running ingress


## TEST AND TROUBLESHOOT

### testing to run apps 
- `kubectl port-forward service name-of-service accessport:insideport`
- `kubectl port-forward svc/service-nginx 8383:8383`

### see logs of running pods
- `kubectl logs namapods`

### if you want use ingress first enable minikube addons
- `minikube addons enable ingress`

### using minikube to make tunnel
- `minikube tunnel`

