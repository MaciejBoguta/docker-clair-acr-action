# docker-clair-acr-action
## GitHub Action that simplifies building a docker image, then scanning it with Clair and finally pushing it to ACR.

## Inputs:
  
* ### image-name  
   (Required) Container repository and image name  
  
* ### tag  
   (Optional) Image tag, defaults to latest
  
* ### should-push-to-acr  
   (Required) Should image be pushed to ACR - "true"/"false"  
   
* ### client-id  
   (Required) Azure client id for authentication to ACR  
   
* ### client-secret  
   (Required) Azure client secret for authentication to ACR  
  
* ### acr-name  
   (Required) ACR instance name  
   
* ### nuget-pat  
   (Optional) Private nuget feed token  
