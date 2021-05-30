# jx3-minikube

Jenkins X 3.x GitOps repository using [minikube](https://minikube.sigs.k8s.io/) to create a kubernetes cluster and local secrets

Check out the [Installation Instructions](https://jenkins-x.io/v3/admin/platforms/minikube/)

## Pre-requisites
 - jx 3.2
 - minikube
 - helm
 - ngrok
 - GitHub
    - Jenkins X cluster GitOps repo
    - Application repo(s)

## Local env on Windows

- Starting the Jenkins X cluster on minikube

```
- minikube start --cpus 4 --memory 8048 --disk-size=100g --addons=ingress --vm=true
- ngrok.exe authtoken <token>
- ngrok.exe http 8080
```

## To view the minikube dashboard
```
 - minikube dashboard
```

##
- Adding new GitHub projects:
 
 ```
  jx.exe import --url <GitHub repo URL>
 ```