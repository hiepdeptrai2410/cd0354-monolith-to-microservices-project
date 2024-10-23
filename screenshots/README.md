# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![alt text](get-pods.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![alt text](describe-services-1.png)
![alt text](describe-services-2.png)
![alt text](describe-services-3.png)
![alt text](describe-services-4.png)
![alt text](describe-services-5.png)
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![alt text](describe-hpa.png)
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![alt text](get-logs.png)

```bash
kubectl get deployments
```
![alt text](get-deployment.png)

```bash
kubectl get services
```
![alt text](get-services.png)

## Docker Images
![alt text](docker-hub.png)

## Travis
![alt text](travis-success.png)