Deploy backend

docker build -t ImagemDoBackend -f Dockerfile .
docker push ImagemDoBackend
kubectl apply -f deployment.yaml


Deploy Mongodb

-kubectl apply mongo-pvc.yaml
-kubectl apply mongo-secrets.yaml
-docker build -t ImagemDaMongoDB -f Dockerfile.db .
-docker push ImagemDaMongoDB
-kubectl apply -f mongo-deployment.yaml
