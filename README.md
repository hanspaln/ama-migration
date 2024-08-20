# ama-migration
This repository will provide step by step process to move from MMA to AMA. Below are the pre-requisites -

1. User Assigned Managed-Identity (UAMI) with Virtual machine contributor role and Log Analytics Workspace contributor
2. Data collection rule to collect the logs of interest and metrics
3. Log Analytics Workspace - Workspace where the logs need to be sent

The migration from MMA to AMA can be automated using Azure Policies. The Poliices will be used to - 

1. Add a VM to the DCR
2. Enable AMA agent
3. Add User Assignment MI to the Virtual Machine

Each of the above activity can be completed using azure policy. The 3 policies can be grouped together and can run within an initiative. 


