# documentation

npx create-react-app my-user-app
npm start

Docker file name is case sensitive "Dockerfile" and with no extension

Commands:

docker login

docker images 

docker build -t myspringmongoreact .
docker build -t reactapp .

docker tag myspringmongoreact codesajith/myspringmongoreact

docker push codesajith/myspringmongoreact

docker rmi myspringmongoreact codesajith/myspringmongoreact

docker run -p 8087:8087 codesajith/myspringmongoreact
docker run -p 3000:3000 reactapp
docker rmi reactapp
docker rmi graalvm-demo


Minisub:

Commands:

Start : minikube start 

status : minikube status

kubectl create deployment springboot-kubernetes --image=codesajith/myspringmongoreact --port=8087

kubectl get deployments

kubectl get pods

kubectl logs <<pod-name from previous command>> 
  eg: kubectl logs springboot-kubernetes-8549dc4c65-c7m6g 

kubectl expose deployment springboot-kubernetes --type=NodePort

kubectl get services

minikube service springboot-kubernetes

kubectl delete service <<my-service>>
 eg:kubectl delete service springboot-kubernetes

kubectl delete deployment springboot-kubernetes

minikube dashboard
