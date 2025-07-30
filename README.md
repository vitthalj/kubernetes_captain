#Commands to create pods for #simple_pod.yaml
#Below are the steps to create a pod for nginx
kubectl create -f simple_pod.yaml

#list all pods with more details 
kubectl get pods -o wide

#command to to watch live actions in a cluster
kubectl get pods -w

#command to to delete a pod in a cluster
kubectl delete pod <pod_name>

#list all replica-sets
kubectl get rs


#Commands to create deployments for #deployment.yaml
#create a deployment 
kubectl apply -f deployment.yaml
