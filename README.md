# SimpleTimeService

A small Python microservice that returns the current time and client IP in JSON format.

## Run locally

pip install -r requirements.txt
python app.py

Open: http://localhost:3000

## Docker

docker build -t techvkm/simple-time-service:latest .
docker push techvkm/simple-time-service:latest

## Kubernetes

kubectl apply -f microservice.yml

kubectl port-forward svc/simple-time-service 8080:80
curl http://localhost:8080
