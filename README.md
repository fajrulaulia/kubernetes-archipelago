# kubernetes archipelago
learning kubernetes in minikube

# Image Defined
- GRPC Service: `faawidia/webservice-grpc:latest`
- Rest API: `faawidia/webapi-rest:latest`
- Simple NodeJS Microservice : `faawidia/simple-nodejs-microservice:latest`


# Before run, install:
- `minikube` and `kubectl`
- `docker`


## Addons
- Enable Ingress = `minikube addons enable ingresss`
- Enable HPA = `minikube addons enable metrics-server`

## Command
- Apply Config:
``` bash 
$ kubectl apply -f filename.yaml  # only apply for filename.yaml 
```
apply for entire yaml file
``` bash 
$ kubectl apply -f filename.yaml 
```

- Get objects:
``` bash 
$ kubectl get developments  # listing deployments
$ kubectl get pods  # listing pods
$ kubectl get services  # listing services for network
$ kubectl get hpa  # listing services for HPA
$ kubectl get ingress  # listing services for ingress
```
for ingress, when you set hostname on config, don't forget to add in host, in linux, adding `/etch/hosts`
- get url 
``` get url 
$ minikube service service_name --url
```

