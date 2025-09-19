# COMMON COMMANDS 

## MINIKUBE

- minikube start
- minikube stop
- minikube ip (returns the virtual machine ip)
- minikube service client-node-port --url
- minikube service ingress-nginx-controller -n ingress-nginx --url

## KUBECTL

- kubectl apply -f client-pod.yaml
- kubectl apply -f client-node-port.yaml
- kubectl get pods
- kubectl get services
- kubectl describe <type> <name>  -  kubectl describe pod client-pod
- kubectl delete <kind_of_object> <object_name> - kubectl delete deployment client-deployment
- kubectl delete -f <file_path> - kubectl delete -f client-pod.yaml
- kubectl set image <object_type> / <object_name> <container_name>=<new_image_to_use>
- kubectl get storageclass
- kubectl get pv - pv = persistente volume
- kubectl get pvc - pvc = persitent volume claims
- kubectl create secret generic pgpassword --from-literal PGPASSWORD=12345asdf
- kubectl get secrets


### NODE

nodes are individual machines or vm's that run containers

## Accessing docker server inside minikube

- eval $(minikube -p minikube docker-env)
