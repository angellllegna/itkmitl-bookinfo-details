# How to run details service
## Prerequisite
* Ruby 2.7
```bash
ruby details.rb 9080
```
## How to run with Docker
```bash
# Build Docker Image for details service
docker build -t details .
# Run ratings service on port 8081
docker run -d --name details -p 8081:8081 details
```
## How to run with Docker Compose
```bash
docker-compose up -d
```
``` 
You can test with path '/health' or '/details/1'
```
## How to run with Kubernetes
```bash
# Create deployment resource
kubectl apply -f k8s/
```