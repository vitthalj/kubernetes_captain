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

#While running these scripts if you get erros like below, you can resolve it using below steps.
error 1.
 Unable to connect to the server: dial tcp [::1]:8080: connectex: No connection could be made because the target machine actively refused it. 

In Windows 10 machine you have to enable kubernetes on docker desktop. go to settings > kubernetes > enable it.
Next you run below command, which will configure the context 
kubectl config get-contexts