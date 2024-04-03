#  How to start minikube on windows
- Chocolatey or Choco as it is sometimes referred to, is a free, open-source package manager for Windows that is very similar to Apt or DNF in the Linux realm.
- Use below command on CMD for installation of choco on windows
    ```bash
	@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command " [System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
- Use below command on CMD for verify the installation of choco on windows
    ```bash
	Choco

    
![minikube](../screenshots/choco_version.PNG?raw=true)