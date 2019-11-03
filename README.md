# Doraemon

####  Set up React Environment
######Building your image

###### switch node mirror to `npm config set registry https://registry.npm.taobao.org` first
###### cd into Doraemon folder, at same level with Dockerfile, run below commands
###### `docker build -t <your username>/react-app .`
###### after building, run `docker image` to check if image exists, then `docker run -p 49160:80 -d <your username>/react-app` to run app in browser
###### then `docker ps` to see daemon process is running, and visit `http://localhost:49160` in browser.


######Building Go image

###### cd into go-docker folder, at same level with Dockerfile, run below commands
###### `docker build -t go-docker .`
###### after building, run `docker image ls` to check if image exists, then `docker run -d -p 8181:8080 go-docker` to run app in browser
###### then `docker ps` to see go process is running

######Install minicube and k8s
minikube start --registry-mirror=https://registry.docker-cn.com --kubernetes-version v1.16.2
minikube start --vm-driver=virtualbox --apiserver-ips 127.0.0.1 --apiserver-name localhost --alsologtostderr -v=8

#### Useful Links
https://nodejs.org/de/docs/guides/nodejs-docker-webapp/

https://medium.com/@shakyShane/lets-talk-about-docker-artifacts-27454560384f

https://www.callicoder.com/docker-golang-image-container-example/s

https://kubernetes.io/docs/tasks/tools/install-minikube/

https://kubernetes.io/docs/tasks/tools/install-kubectl/


