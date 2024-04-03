#  How to start minikube on windows
- Add repo Prometheus to helm:
    ```bash
	helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

- Install helm chart for Prometheus:
    ```bash
	helm install prometheus prometheus-community/prometheus

- Create the service name and expose port no:
    ```bash
	kubectl expose service prometheus-server --type=NodePort --target-port=9090 --name=prometheus-server-np

![minikube](../screenshots/prome_svc.PNG?raw=true)

- Check status of the pods:
    ```bash
	kubectl get pods -l app.kubernetes.io/instance=prometheus
    
![minikube](../screenshots/prome_pods.PNG?raw=true)

- Hit the browser once all the pods are up and running:
    ```bash
	minikube service prometheus-server-np


