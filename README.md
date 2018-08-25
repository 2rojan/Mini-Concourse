This is a work in progress and gets you to a running state (meaning you can bring the UI up via brower and login).
It is not however fully tested.

To generate your keys, see https://concourse.ci/docker-repository.html and https://concourse.ci/binaries.html 
for notes on getting started.

Also see https://github.com/kubernetes/minikube/releases/tag/v0.12.1 for notes regarding minikube.

In this example, minikube was run on OSX sierra with v0.12.1 and xhyve hypervisor.

Minikube cluster created with `minikube start --vm-driver=xhyve`

Order for which to create specs with k8s.

1. concourse-ns.yml
2. concourse-db-deployment.yml
3. concourse-db-svc.yml
4. concourse-web-secrets.yml
5. concourse-web-deployment.yml
6. concourse-web-svc.yml
7. concourse-worker-secrets.yml
8. concourse-worker-deployment.yml