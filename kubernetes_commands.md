** All Kubernetes commands **
- kubectl create -f .\deploy_initial.yaml 
- kubectl apply -f .\deploy_initial.yaml 
- kubectl get pods
- kubectl get pods -o wide
- kubectl logs -f initiallocalapp
- kubectl delete pod initiallocalapp
- minikube dashboard
kubectl get pods --show-labels

to run your lcoal docker images

minikube docker-env
minikube -p minikube docker-env --shell powershell | Invoke-Expression


kubectl describe rc replication-controller-demo
kubectl scale --replicas=1 rc -l app=replication-controller-demo
kubectl delete rc replication-controller-demo
kubectl get rs
kubectl delete rs replicaset-demo