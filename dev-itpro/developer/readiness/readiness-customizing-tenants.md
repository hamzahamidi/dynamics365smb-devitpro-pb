---
title: "Customizing Tenants"
description: ""
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 04/01/2021
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: conceptual
ms.service: "dynamics365-business-central"
ms.author: solsen
---

# Customizing Tenants

Every business is unique. Harness the power of [!INCLUDE[d365_bus_central_md](../includes/d365_bus_central_md.md)] to match how you work: your streamlined processes, your terminology, and how your employees or departments connect and collaborate.  

Whilst there may already be Add-on apps available on AppSource that cover a customer’s need, we’ve also have the tools for you to build fully custom functionality or adapt what is already available out-of the box. 
 
## Examples of custom changes to [!INCLUDE[d365_bus_central_md](../includes/d365_bus_central_md.md)] 

- Capture industry-specific information about the products you sell. 
- Connect to other in-house data repositories or legacy systems to reduce duplicate data entry. 
- Hide data fields that are rarely or never used. 
- Add a printable report covering legally required declarations for your industry. 
- Create a role-specific dashboard and set of tasks for a unique role in your organization, such as mobile purchasing managers, or recruiting specialists. 
 
## How do I customize? 

For most simple changes, the browser-based Designer allows you to rapidly adjust the UI without needing to write any code. Hide columns you don’t need, drag-and-drop to reposition FactBoxes, or show data fields that were previously hidden: these are all examples of simple changes you can roll out to your entire organization using Designer. For more information, see [Using Designer](../devenv-inclient-designer.md)

With Visual Studio Code and the [!INCLUDE[d365al_ext_md](../../includes/d365al_ext_md.md)], you’re able to customize existing pages and tables by creating page and table extensions, or you can add new tables and pages to make entirely new functionality. You can even write business logic in AL. For more information, see [Getting Started with AL](../devenv-get-started.md).

You can start customizing in either Designer or in Visual Studio Code. If you start in Designer, the AL source code generated by the designer is downloadable, so you can continue developing in Visual Studio Code if needed. If you start developing in Visual Studio Code, you will initiate Designer directly from Visual Studio Code, to customize using Designer. When done using Designer you synchronize changes back to Visual Studio code keeping all changes reflected in the AL source code.  

The resulting AL code is compiled into an .app file, which can be deployed to production tenants. 

## How do I test my custom changes? 

To ensure business continuity and protect the integrity of live customer data, you cannot customize [!INCLUDE[d365_bus_central_md](../includes/d365_bus_central_md.md)] for an organization running in production. Instead, custom changes are tested on hosted sandbox environments or in Docker containers. Changes can be tested thoroughly in the browser until they are deemed fit to deploy into production where they are applied as an app and can immediately be used by everyone in the organization. 

## Where do I learn more? 

To learn more about customization, select the following links:  

- [Using Designer](../devenv-inclient-designer.md)  
- [Getting started with AL](../devenv-get-started.md)  
- [AL Development Environment](../devenv-reference-overview.md)  
- [Business Central Learning Catalog](/dynamics365/business-central/readiness/readiness-learning-catalog)