#  How to start minikube on windows and Ubuntu
- Start the Minikube 
    - ```bash
        minikube start
    
 - This will take some time, if you are facing some error related to hypervisor, you can below command.
    - ```bash
        minikube start --driver=virtualbox --no-vtx-check
      - OR
        minikube start --driver=virtualbox --force
    
![minikube](../screenshots/minikube_start.PNG?raw=true)
