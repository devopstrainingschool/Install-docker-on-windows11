# Install-docker-on-windows11
## Make sure that you open a terminal as administrator:
![image](https://user-images.githubusercontent.com/107158398/223482894-ca1b77ec-e90a-480f-a2ef-46539f880f11.png)

## Install chocolatey 
### Please use one of these two options depending on the terminal.
### 1- Wih cmd terminal:
```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```
### 2- With powershell terminal:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
## Install docker on windows 11
### Please run this command
```
choco install docker-desktop
```
### let check if docker is installed:
```
docker version
```


