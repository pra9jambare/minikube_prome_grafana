#   Install Kubectl for windows
- Download the kubectl from documentation. [\[Click Here\]](https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/) to visit windows installation
- Install the kubectl.exe 
- Add Minikube to the PATH environment variable
- System --> Advanced System Settings --> Environment Variable --> Path --> Edit --> New --> OK 
- Open the Command Prompt and type “kubectl version”. This should display the version of kubectl that you have installed.
![minikube](../screenshots/kubectl_version.PNG?raw=true)
	
# Install Kubectl for Ubuntu
- Update System and Install Required Packages
     ``` bash
    sudo apt-get update -y
    ```
    ``` bash
    sudo apt-get upgrade -y
    ```
    ``` bash
    sudo apt-get install curl
    ```
    ``` bash
    sudo apt-get install apt-transport-https
    ```


- Download kubectl 
    ``` bash
    curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
    ```
- Make the binary executable
    ``` bash
    chmod +x ./kubectl
    ```
- move the binary into local binary directory
    ``` bash
    sudo mv ./kubectl /usr/local/bin/kubectl
    ```
- Verify the installation by checking the version 
    ``` bash
    kubectl version -o json
    ```


#   Install Hypervisor for Windows
- Download the virtual box from documentation. [\[Click Here\]](https://www.virtualbox.org/wiki/Downloads) to visit windows installation
- Install the virtual box 

# Install Hypervisor for Ubuntu
- To install VirtualBox on Ubuntu 
    ``` bash
    sudo apt install virtualbox virtualbox-ext-pack
    ```
    - Press 'y' and hit Enter to confirm the installation.
    - Use Tab to navigate to the license agreement, then hit Enter to proceed.
    - Select 'Yes' to agree with the terms of the VirtualBox PUEL license when prompted by the installer.
    - Wait for the installation to finish before proceeding to the next step.
    


#   Install Minikube for Windows
- Download the Minikube from Github. [\[Click Here\]](https://github.com/kubernetes/minikube/releases/) to visit repository
- Install the Minikube.exe 
- Add Minikube to the PATH environment variable
- System --> Advanced System Settings --> Environment Variable --> Path --> Edit --> New --> OK 
- Open the Command Prompt and type “minikube version”. This should display the version of Minikube that you have installed
![minikube](../screenshots/minikube_version.PNG?raw=true)

# Install Minikube for Ubuntu
- Use wget to download the most recent Minikube binary.
    ``` bash
    wget https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
    ```
- Paste the downloaded file into the /usr/local/bin/minikube directory.
    ``` bash
    sudo cp minikube-linux-amd64 /usr/local/bin/minikube
    ```
- Grant executable permissions to the file within the minikube directory.
    ``` bash
    sudo chmod 755 /usr/local/bin/minikube
    ```
- Confirm the successful installation of Minikube by checking its version.
    ``` bash
    minikube version
    ```