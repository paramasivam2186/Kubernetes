#  TestNG Parallel with Kubernetes

[comment]: <> (minikube start --driver=virtualbox)

[comment]: <> (wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb)

[comment]: <> (wget https://chromedriver.storage.googleapis.com/2.37/chromedriver_linux64.zip)

[comment]: <> (kubectl create -f selenium-hub-deployment.yaml)

[comment]: <> (kubectl get all -l name=selenium-hub)

[comment]: <> (kubectl expose deployment selenium-hub-deployment --type=NodePort --port=4444)

[comment]: <> (minikube service selenium-hub-deployment --url)

[comment]: <> (kubectl create -f selenium-node-chrome-deployment.yml)

[comment]: <> (kubectl scale deployment.apps/selenium-node-chrome-deployment --replicas=2)

[comment]: <> (kubectl get pods)

[comment]: <> (kubectl delete --all deployments)

[comment]: <> (kubectl delete --all services)

[comment]: <> (kubectl get all)