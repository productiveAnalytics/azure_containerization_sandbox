# Azure Container Instances (ACI)

Login to Azure Cloud Shell
```git clone https://github.com/Azure-Samples/aci-helloworld.git```
```cd aci-helloworld```
Open built-in VS code: ```code .```
Update index.html and Save
Ensure that Azure Container Registry (ACR) exists: myacr
Build new docker image and upload to ACR: ```ACR build commands goes here```
Create new ACI with the custom image from the ACR
Note the public IP of the ACI
On Cloud Shell, ```curl -X GET <public-ip-of-ACI>```