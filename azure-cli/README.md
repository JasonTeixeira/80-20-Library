# Azure CLI: 80/20 Essential Command Library

## Overview
The Azure CLI is a powerful tool that allows engineers to manage Azure resources directly from the command line. The commands in this section adhere to the **80/20 principle**, focusing on the most critical operations for managing compute, networking, storage, and other Azure services.

---

## 1. Virtual Machines (VM)
- `az vm list` – List all virtual machines in the subscription.
- `az vm start --name <vm-name> --resource-group <group>` – Start a VM.
- `az vm stop --name <vm-name> --resource-group <group>` – Stop a VM.
- `az vm delete --name <vm-name> --resource-group <group> --yes` – Delete a VM.
- `az vm show --name <vm-name> --resource-group <group>` – Show VM details.

---

## 2. Storage Accounts
- `az storage account list` – List all storage accounts.
- `az storage account create --name <account-name> --resource-group <group>` – Create a new storage account.
- `az storage blob upload --account-name <account> --container-name <container> --file <file-path>` – Upload a blob to a container.
- `az storage blob list --account-name <account> --container-name <container>` – List blobs in a container.
- `az storage account delete --name <account-name> --resource-group <group>` – Delete a storage account.

---

## 3. Networking
- `az network vnet list` – List all virtual networks.
- `az network vnet create --name <vnet-name> --resource-group <group>` – Create a new virtual network.
- `az network nsg list` – List all network security groups.
- `az network nsg create --name <nsg-name> --resource-group <group>` – Create a network security group.
- `az network public-ip list` – List all public IP addresses.

---

## 4. Resource Groups
- `az group list` – List all resource groups.
- `az group create --name <group-name> --location <location>` – Create a new resource group.
- `az group delete --name <group-name> --yes --no-wait` – Delete a resource group.
- `az group show --name <group-name>` – Show details about a resource group.

---

## 5. Monitoring and Logs
- `az monitor metrics list --resource <resource-id>` – List metrics for a resource.
- `az monitor alert list` – List all alerts.
- `az monitor log-analytics workspace list` – List Log Analytics workspaces.
- `az monitor log-analytics query --workspace <workspace-id> --analytics-query "<query>"` – Run a query in Log Analytics.

---

## 6. Identity and Access Management (IAM)
- `az ad user list` – List all Azure Active Directory users.
- `az role assignment list --assignee <user>` – List role assignments for a user.
- `az role assignment create --assignee <user> --role <role>` – Assign a role to a user.
- `az ad group create --display-name <group-name> --mail-nickname <nickname>` – Create a new AD group.

---

## Conclusion
These **Azure CLI commands** cover the majority of tasks involved in managing Azure resources. Mastering these commands will significantly improve your efficiency and help you manage Azure environments effectively, from virtual machines to networking and storage services.

---


