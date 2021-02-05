# Terraform on Azure Cloud 

## Prerequisites

1. Install azcli
2. Install Terraform

Optional :
Create a Service Principal (ad sp)


```bash
# Get Subscription ID
az ad account show

# Create Service Principal

az ad sp create-for-rbac -n "IACSP" --role Contributor --scopes  /subscriptions/"XXXXXX-xxxx-xxxx-xxx-xxxxxxxxx"/
```      

```json
{
  "appId": ""XXX-XXXX-XXXXXX-XXX"",
  "displayName": "IACSP",
  "name": "http://IACSP",
  "password": ""XXX-XXXX-XXXXXX-XXX"",
  "tenant": ""XXX-XXXX-XXXXXX-XXX""
}




```
```bash
 export ARM_CLIENT_ID="XXX-XXXX-XXXXXX-XXX"
 export ARM_CLIENT_SECRET="XXX-XXXX-XXXXXX-XXX"
 export ARM_SUBSCRIPTION_ID="XXX-XXXX-XXXXXX-XXX"
 export ARM_TENANT_ID="XXX-XXXX-XXXXXX-XXX"
```



"tenantId": "XXX-XXXX-XXXXXX-XXX",
"id": "XXXX-XXX-XXX-XXXX-XXXXX"


## Types of blocks

1. providers
2. resources
3. variables
4. data
5.outputs



```bash
terraform init
terraform plan
```
