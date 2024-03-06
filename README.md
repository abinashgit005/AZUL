# AZUL

## step 1
Manually created a resourcegroup and storage account for terraform backend (this can be created in terraform as well.)

I have implemented IAC with Terraform to create a resourcegroup and storage account for saving the data.
```yaml
# providers details

terraform {
  required_providers {
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "=3.0.0"
    }
  }
}
# terraform backend
terraform {
  backend "azurerm" {}
}

provider "azurerm" {
  features {}
}
```
> [!WARNING]
> got below error while trying to variablize the resource group name and location, So tried to keep it simple.

![image](https://github.com/abinashgit005/AZUL/assets/78551736/e5f210ef-b7f0-445f-bc05-008a7df05f66)
