# Doraemon

####  Set up Environment
######Building your image

###### switch node mirror to `npm config set registry https://registry.npm.taobao.org` first
###### cd into Doraemon folder, at same level with Dockerfile, run below commands
###### `docker build -t <your username>/react-app .`
###### after building, run `docker image` to check if image exists, then `docker run -p 49160:80 -d <your username>/react-app` to run app in browser
###### then `docker ps` to see daemon process is running, and visit `http://localhost:49160` in browser.

#### Useful Links
https://nodejs.org/de/docs/guides/nodejs-docker-webapp/

https://medium.com/@shakyShane/lets-talk-about-docker-artifacts-27454560384f

https://www.callicoder.com/docker-golang-image-container-example/
