---
title: "Use the Dynamics 365 for Customer Engagement apps (online) service admin role to manage your tenant | MicrosoftDocs"
ms.custom: 
ms.date: 05/16/2019
ms.reviewer: 
ms.service: crm-online
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
applies_to: 
  - Dynamics 365 for Customer Engagement  (online)
  - Dynamics 365 for Customer Engagement  Version 9.x
ms.assetid: a92f7d58-fbe0-4ad7-bf42-d2961e306b85
caps.latest.revision: 4
author: jimholtz
ms.author: jimholtz
manager: kvivek
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - Powerplatform
---
# Use the service admin role to manage your tenant 

[!INCLUDE[cc-applies-to-update-9-0-0](../includes/cc_applies_to_update_9_0_0.md)]

To help you administer [!INCLUDE[pn_dyn_365_online](../includes/pn-crm-online.md)], you can assign users to manage [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] at the tenant level without having to assign the more powerful [!INCLUDE[pn_Office_365](../includes/pn-office-365.md)] global admin privileges.  
  
 Users with the [!INCLUDE[pn_dyn_365_online](../includes/pn-crm-online.md)] service admin role can:  
  
- Sign in to and manage  multiple [!INCLUDE[pn_dyn_365_online](../includes/pn-crm-online.md)] instances. If an instance uses a security group, a service administrator would need to be added to the security group in order to manage that instance.  
  
- Perform admin functions in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] because they have the [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] system admin role. The service admin must be assigned a [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] license.  
  
A [!INCLUDE[pn_dyn_365_online](../includes/pn-crm-online.md)] service admin cannot do functions restricted to the [!INCLUDE[pn_Office_365](../includes/pn-office-365.md)] global admin such as manage user accounts, manage subscriptions, access settings for [!INCLUDE[pn_Office_365](../includes/pn-office-365.md)] apps like [!INCLUDE[pn_Exchange](../includes/pn-exchange.md)] or [!INCLUDE[pn_SharePoint_short](../includes/pn-sharepoint-short.md)].  
  
> [!NOTE]
> The [!INCLUDE[pn_dyn_365_online](../includes/pn-crm-online.md)] service admin can manage instances of version 8.1 ([!INCLUDE[pn_crm_8_1_0_online](../includes/pn-crm-8-1-0-online.md)]) or later.  
  
 ![Dynamics 365 service admin](../admin/media/dynamics-365-service-admin.png "Dynamics 365 service admin")  
  
 Here's a matrix of what's available with the various [!INCLUDE[pn_Office_365](../includes/pn-office-365.md)] roles.  
  
|Office 365 role / feature|Backup & restore|Sandbox copy|Configure new instances|Manage an instance|Add Customer Engagement licenses|Access support requests|Access Service health|Access Message center|  
|--------------------------------|----------------------|------------------|-----------------------------|------------------------|-------------------------------|---------------------------------|-----------------------------|---------------------------|---------------------------|  
|Office 365 global admin|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|  
|Exchange admin|n/a|n/a|n/a|n/a|n/a|n/a|Yes|Yes|  
|Office 365 service admin|No|No|No|No|No|Yes|Yes|Yes|  
|Office 365 user|No|No|No|No|No|No|No|No|  
|Dynamics 365 service admin|Yes|Yes|Yes|Yes|No|Yes|Yes|Yes| 
|License administrator|No|No|No|No|Yes|No|No|No|  

> [!NOTE]
> For information on email approval, see [Approve email](connect-exchange-online.md#approve-email).

### See also  
 [Manage Microsoft Dynamics 365 for Customer Engagement apps (online) instances](../admin/manage-online-instances.md)   
 [Manage subscriptions, licenses, and user accounts](../admin/manage-subscriptions-licenses-user-accounts.md)