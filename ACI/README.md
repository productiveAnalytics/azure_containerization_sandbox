# Azure Container Instances (ACI)

1. Login to Azure Cloud Shell
2. ```git clone https://github.com/Azure-Samples/aci-helloworld.git```
3. ```cd aci-helloworld```
4. Open built-in VS code: ```code .```
5. Update index.html and Save
6. Ensure that Azure Container Registry (ACR) exists: myacr
7. Build new docker image and upload to ACR: ```ACR build commands goes here```
8. Create new ACI with the custom image from the ACR
9. Note the public IP of the ACI
10. On Cloud Shell, ```curl -X GET <public-ip-of-ACI>```
