# aadRoleSync
Welcome to the aadRoleSync repo

aadRoleSync provides a means to manage Azure AD Roles with on-prem Active Directory groups.  It does this by syncrhonising on-prem AD groups with AAD groups which in turn have been assigned to Azure AD roles.  aadRoleSync is written in C# and utilizes the Graph API to interact with Azure AD.  It is written as a Azure Function which is scheduled to run on a timer.

The intention of aadRoleSync is to make managing AAD Roles easier.  It is aimed at entities that have mature processes for managing on-prem AD group membership, leveraging established processes and good goverence that can easily be extended to AAD Roles.

## Warning
If you do not have good security practicies around managing on-prem security groups then stop now, aadRoleSync is not for you, don't risk exposing your AAD Roles, instead spend your time improving your on-prem security posture!! 

# Requirements
There are a few things you'll need to be able to leverage aadRoleSync;
## Fundamentals
- AAD Connect - you must sync your on-prem AD into Azure AD
- An Azure Subscription - aadRoleSync runs as an Azure FUnction, you'll need an Azure subscription
## Setup Requirements
- You'll need a Global Admin account for setup - this is ONLY needed to carry out the setup steps that follow, you'll delegate some Graph API rights to a Service Princpal that aadRoleSync will use on an ongoing basis, aadRoleSync does not require Global Admin rights itself.
- Permission to create on-prem AD groups
- Rights to setup and deploy to an Azure Function App, Azure Storage, Azure Key Vault.
- Azure AD Preview PowerShell Module
- Az PowerShell Module

# aadRoleSync Overview


# Getting Started
### 1.  Clone the Repo!
### 2.  Setup Groups
### 3.  Setup Service Principal
### 4.  Deploy Function App
