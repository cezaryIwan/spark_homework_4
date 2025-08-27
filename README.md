# Setup of infrastructure
1. Created a resource group with <br>
`az group create --name sparkhm4 --location polandcentral`<br>
2. Created storage account with<br>
`az storage account create --name sasparkhm4 --resource-group sparkhm4 --location polandcentral --sku Standard_LRS`<br>
4. Created storage container with<br>
`az storage container create --name contsparkhm4 --account-name sasparkhm4`<br>
4. Updated terraform configuration in main.tf<br>
5. Deployed infrastructure with<br>
`terraform init && terraform plan -out terraform.plan && terraform apply terraform.plan`<br>
# Few screenshots
Final result:<br>
<img width="1711" height="905" alt="image" src="https://github.com/user-attachments/assets/bcfb1572-5591-44f7-805c-b1567ea1104a" /><br>
Runs:<br>
<img width="1429" height="864" alt="image" src="https://github.com/user-attachments/assets/906a78eb-068e-4e7f-b280-3149a6440caa" /><br>
Models:<br>
<img width="1507" height="371" alt="image" src="https://github.com/user-attachments/assets/b04e085f-08f6-4664-8ea1-de49122a95e3" /><br>
Serving endpoint:<br>
<img width="1344" height="828" alt="image" src="https://github.com/user-attachments/assets/8974a9da-7052-4560-ab79-8ea7f5011437" /><br>
