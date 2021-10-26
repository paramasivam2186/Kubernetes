#  TestNG Parallel with Kubernetes
# minikube start --driver=virtualbox
# wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
# wget https://chromedriver.storage.googleapis.com/2.37/chromedriver_linux64.zip
# kubectl create -f selenium-hub-deployment.yaml
# kubectl get all -l name=selenium-hub
# kubectl expose deployment selenium-hub-deployment --type=NodePort --port=4444
# minikube service selenium-hub-deployment --url
# kubectl create -f selenium-node-chrome-deployment.yml
# kubectl scale deployment.apps/selenium-node-chrome-deployment --replicas=2
# kubectl get pods
# kubectl delete --all deployments
# kubectl delete --all services
# kubectl get all