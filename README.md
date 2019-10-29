# refactor-udagram-app-into-microservices-and-deploy
Udacity Cloud Developer Nanodegree Program - project  4


## About Project:
goal of project to create web app that user can register and log-gin and upload images to S3 bucket, then show images (even when user is not logged-in)

## Technical Info:
project has docker-compose file to run docker containers, each docker container has pne service whcih are : frontend service, rest API user service, and rest API feed service. both user and feed use the same port and reverseproxy control the incoming traffic between them.

Also, the project has kubernete which run each docker dontainer inside pod in cluster.


1- run docker compose 
docker-compose up

2- port-forward 
kubectl port-forward service/frontend 8100:8100
kubectl port-forward service/reverseproxy 8080:8080

