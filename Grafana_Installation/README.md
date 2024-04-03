#  How to install Grafana using Helm
- Add repo Grafana to helm:
    ```bash
	helm repo add grafana https://grafana.github.io/helm-charts 

- Install helm chart for Grafana:
    ```bash
	helm install grafana grafana/grafana

- Create the service name and expose port no:
    ```bash
	kubectl expose service grafana --type=NodePort --target-port=3000 --name=grafana-np 

![minikube](../screenshots/grafana_svc.PNG?raw=true)

- Check the username & password for Grafana :
    ```bash
	kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}"
- Decode the password with base64 

![minikube](../screenshots/grafana_pod.PNG?raw=true)

- Hit the browser once all the pods are up and running:
    ```bash
	minikube service grafana-np
