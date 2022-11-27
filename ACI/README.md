# Azure Container Instances (ACI)

1. Login to Azure Cloud Shell
- If needed check the persistent storage associated with Cloud Shell, switch to PowerShell instead of Bash and run: ```Get-CloudDrive```
- To update persistent storage and/or file-share: ```Dismount-CloudDrive``` and configure interactively
2. ```git clone https://github.com/Azure-Samples/aci-helloworld.git```
3. ```cd aci-helloworld```
4. Open built-in VS code: ```code .```
5. Update index.html and Save
6. Ensure that Azure Container Registry (ACR) exists: *myacr*
7. Build new docker image with tag v1 and upload to ACR: ```az acr build --image aci-demo/custom-image-demo:v1 --registry myacr --file Dockerfile . ```
8. Create new ACI with the custom image from the ACR
9. Note the public IP of the ACI
10. On Cloud Shell, ```curl -X GET <public-ip-of-ACI>```
