#  Create a deployment with blue - green strategy
- What is Blue Green Deployment:>
   - Deployment strategy in which you create two separate, but identical environments.
   - Mainly this strategy is used for maintenance purpose.

- Create a deployment of a simple application.
  - Find the deployment yaml [here](https://github.com/pra9jambare/minikube_prome_grafana/tree/main/Deploy_App_with_Blue_Green/)

- Provide 3 replicas (It can vary as per your requirement) 

- Create Blue & Green deployment
  - Find the blue deployment yaml [here](https://github.com/pra9jambare/minikube_prome_grafana/tree/main/Deploy_App_with_Blue_Green/blue_deploy.yaml)
  - Find the green deployment yaml [here](https://github.com/pra9jambare/minikube_prome_grafana/tree/main/Deploy_App_with_Blue_Green/green_deploy.yaml)

  ![grafana](../screenshots/blue_green_pod.PNG?raw=true)

- Create Blue & Green service
  - Find the blue service yaml [here](https://github.com/pra9jambare/minikube_prome_grafana/tree/main/Deploy_App_with_Blue_Green/blue_svc.yaml)
  - Find the green service yaml [here](https://github.com/pra9jambare/minikube_prome_grafana/tree/main/Deploy_App_with_Blue_Green/green_svc.yaml)

![grafana](../screenshots/blue_green_svc.PNG?raw=true)


- Monitor deployment using Grafana and Prometheus

![grafana](../screenshots/grafana_dash.PNG?raw=true)