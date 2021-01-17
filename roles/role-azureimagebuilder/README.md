# Azure Image Builder Managed Identity and Role

## Overview

This template creates the Managed Identity, the corresponding role, and the role
assignment as defined in the [Azure Image Builder
documentation](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/image-builder-permissions-cli#custom-image-azure-role-example).

The template uses the following three parameters:

* aibIdentityName
* roleName
* roleDescription

The defaults for the parameters are set in parameters.json but can be
overrode at runtime.

## Deployment

Deploying this template via the CLI is straight forward.

An example using the default parameters is below:

```bash
az deployment group create -g rg-eastus-aib -n role-azureimagebuilder -p @./parameters.json -f ./deploy.json
```
