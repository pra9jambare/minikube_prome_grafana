#  How to start minikube on windows
- Run below command on CMD
    ```bash
	choco install kubernetes-helm

- Use below command on CMD for verify the installation of helm on windows
    ```bash
	helm version

![minikube](../screenshots/helm_version.PNG?raw=true)


#  How to start minikube on windows
- Download the binary using wget.
    ```bash
	wget -O helm.tar.gz https://get.helm.sh/helm-v3.13.0-rc.1-linux-amd64.tar.gz

- Extract the downloaded file.
    ```bash
	tar -zxvf helm.tar.gz

- Move the helm executable to the bin directory.
    ```bash
	sudo mv linux-amd64/helm /usr/local/bin/helm

- Validate by executing the helm command.
    ```bash
    helm

    
