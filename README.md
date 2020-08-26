# Tika with k8s

### Prerequisite
* [Docker](https://www.docker.com/)
* [Kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
* [Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)
TLDR; You need to know how to run kubernetes:)

### How to start locally
* run `cd tika`
* run `kubectl apply -f .`
* run `minikube ip` and get the ip address. 
  * You will get something like 172.17.48.35
* open `curl -X GET 172.17.48.35:30001` to see welcome page. 
* run `curl -X GET 172.17.48.35:30001/tika`. 
  * It should return something like "This is Tika Server (Apache Tika 1.24.1). Please PUT".