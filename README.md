# refactor-udagram-app-into-microservices-and-deploy
Udacity Cloud Developer Nanodegree Program - project  4

1- run docker compose 
docker-compose up

2- port-forward 
kubectl port-forward service/frontend 8100:8100
kubectl port-forward service/reverseproxy 8080:8080
