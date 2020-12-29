# ansible
Ansible Playground

## Azure DPS Provisioning
### Install Ansible
sudo apt-get install ansible </br>
### Install Azure CLI
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash </br>

// Get the subscription ID registered </br>
az login </br>
az account list --query [*].[name,id] </br>
az ad sp create-for-rbac --role="Contributor" --scopes="/subscriptions/<$subscriptionid>" </br>

export AZURE_SUBSCRIPTION_ID=8d026bb1-..... </br>
export AZURE_TENANT=9f340302-.............. </br>
export AZURE_CLIENT_ID=f86af23a-........... </br>
export AZURE_SECRET=37d908aa-.............. </br>

