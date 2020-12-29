# ansible
Ansible Playground

## Azure DPS Provisioning
### Install Ansible
sudo apt-get install ansible </br>
### Install Azure CLI
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash </br>

Create credentials file inside .azure folder in home directory having service principal content </br>

// Get the subscription ID registered </br>
az login </br>
az account list --query [*].[name,id] </br>
az ad sp create-for-rbac --role="Contributor" --scopes="/subscriptions/<$subscriptionid>" </br>

