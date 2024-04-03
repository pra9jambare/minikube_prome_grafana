#  How to configure Grafana with Prometheus
- Ideally the URL for the Prometheus will be <minikube_ip>:<nodeport_ip>
    ```bash
	http://192.167.39.115:30235/Graph

- Copy the URL and login to Grafana with password obtained while installation

- Go to Connection --> Add New Data Source --> Select Prometheus
![minikube](../screenshots/connection_prome.PNG?raw=true)

- Provide the name for the source code, Paste Prometheus URL in soruce code URL
![minikube](../screenshots/configure_prome.PNG?raw=true)

- Check and Test the connectivity

- You can import or design the visualization as per your requirement
  - Dashboard --> Import --> URL or Id 
  - You can use “6417“ Id  

- You can find the dashboard list under Home --> Dashboard

![minikube](../screenshots/grafana_dash_list.PNG?raw=true)