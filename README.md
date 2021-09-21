# docker-clair-acr-action
GitHub Action that simplifies building a docker image, then scanning it with Clair and finally pushing it to ACR.

Inputs:
  
  image-name:
    description: "Container repository and image name"
    required: true

  tag:
    description: "Image tag, defaults to latest"
    required: false
    default: "latest"

  should-push-to-acr:
    description: "Should image be pushed to ACR"
    required: true

  client-id:
    description: "Azure client id for authentication to ACR"
    required: true

  client-secret:
    description: "Azure client secret for authentication to ACR"
    required: true

  acr-name:
    description: "ACR instance name"
    required: true

  nuget-pat:
    description: "Private nuget feed token"
    required: false