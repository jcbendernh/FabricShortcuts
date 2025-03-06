# Introduction

Contributors to this repo are [Zachary Christoff](https://www.linkedin.com/in/zach-christoff-485b7466/) and myself.

The purpose of this repository is to offer guidance / instruction on how to secure specific tables in a Fabric Lakehouse so that a subset of users can access only those tables and not have access to entire Lakehouse on the Target Path.

This scenario came up repeatedly across customers and we decided to publicly document the steps we have taken to achieve this scenario.

It is also important to note, that when utilizing a medallion Lakehouse model, wee also recommend not putting everything in one workspace.  A good foundation to work with is the following...

![Workspace Best Practices](./img/wrkspcbest1.png)

![Workspace Best Practices](./img/wrkspcbest2.png)

Depending on your scenario, you may need to deviate from this but this is a good place to get started and then adjust as needed.

# Scenario
## Overview
Zach Christoff is a Fabric user who need access to only specific tables that reside the in the Curated Workspace.  We want to create a separate workspace and allow him to access only a few tables.

## Users Involved 
<B>Jack Bender</B> – Admin User, is Admin in both workspaces<br>
<B>Zach Christoff</B> - Power BI User, no admin rights, only has access the US Partners workspace.

## Glossary
<B>Target path</B>: The location that a shortcut points to.
<B>Shortcut path</B>: The location where the shortcut appears
This aligns with the nomenclature at [Secure and manage OneLake shortcuts - Microsoft Fabric | Microsoft Learn](https://learn.microsoft.com/en-us/fabric/onelake/onelake-shortcut-security)







