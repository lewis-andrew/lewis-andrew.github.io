---
title: "Migrate your Unified Service Desk for Dynamics 365 for Customer Engagement apps configuration to another Dynamics 365 for Customer Engagement apps instance | MicrosoftDocs"
description: "Learn how to move a Unified Service Desk for Dynamics 365 for Customer Engagement apps configuration to another instance."
ms.custom: 
  - dyn365-USD, dyn365-admin
ms.date: 08/23/2017
ms.reviewer: 
ms.service: dynamics-365-customerservice
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
applies_to: 
  - Dynamics 365 for Customer Engagement apps
  - Dynamics 365 for Customer Engagement (on-premises) apps
  - Dynamics CRM 2013
  - Dynamics CRM 2015
  - Dynamics CRM 2016
ms.assetid: 49ebffe9-a55c-466a-a5ea-779510db2c4f
caps.latest.revision: 7
author: kabala123
ms.author: kabala
manager: shujoshi
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - D365USD
---
# Migration of a Unified Service Desk configuration 
After you have completed the development or configuration of your agent application, you might want to migrate your latest [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] configuration data from your development or testing environment to your production environment. Migrating your data involves exporting your existing configuration data from the source [!INCLUDE[pn_crm_shortest](../../includes/pn-crm-shortest.md)] instance, and then importing it into the target [!INCLUDE[pn_crm_shortest](../../includes/pn-crm-shortest.md)] instance.  
  
 To export your configuration data, you can use the [!INCLUDE[pn_configuration_migration_tool](../../includes/pn-configuration-migration-tool.md)] and the default [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] configuration data schema file (USDDefaultSchema.xml). The default schema file contains information about all the [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] entities, relationships, and uniqueness definitions for each entity. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Export Unified Service Desk configuration data](../../unified-service-desk/admin/export-unified-service-desk-configuration-data.md)  
  
 For more information about the [!INCLUDE[pn_configuration_migration_tool](../../includes/pn-configuration-migration-tool.md)], see [Manage your configuration data](/dynamics365/customer-engagement/admin/manage-configuration-data).  
  
> [!NOTE]
>  The default [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] configuration data schema file does not export user information from the source system.  
> 
>  For records that include notes and attachments, including Customization Files (compressed folder), these items aren’t included in the record during the export.  
  
 To import the exported [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] configuration data to a [!INCLUDE[pn_crm_shortest](../../includes/pn-crm-shortest.md)] instance, you can do either of the following:  
  
- **Use the Configuration Migration tool**: The tool also enables you to import the exported configuration data. Before you do that though, you must deploy one of the sample [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] packages to create the underlying entities in the target [!INCLUDE[pn_crm_shortest](../../includes/pn-crm-shortest.md)] instance. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Import configuration data using the Configuration Migration tool](../../unified-service-desk/admin/import-unified-service-desk-configuration-data.md#ConfigMigration)  
  
- **Use a custom package for Unified Service Desk**: Create a custom package for [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] to include the exported data along with the files in one of the sample [!INCLUDE[pn_unified_service_desk](../../includes/pn-unified-service-desk.md)] packages, and then deploy the custom package on the target [!INCLUDE[pn_crm_shortest](../../includes/pn-crm-shortest.md)] instance using the [!INCLUDE[pn_package_deployer_tool](../../includes/pn-package-deployer-tool.md)]. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Import configuration data using a custom package for Unified Service Desk](../../unified-service-desk/admin/import-unified-service-desk-configuration-data.md#CustomPackage)  
  
> [!IMPORTANT]
>  The [!INCLUDE[pn_configuration_migration_tool](../../includes/pn-configuration-migration-tool.md)] provides logging support to record detailed information about:  
> 
> - Errors that can occur while signing in to the [!INCLUDE[pn_microsoftcrm](../../includes/pn-microsoftcrm.md)] apps instance using the tool.  
> - Activities performed by the tool during the schema definition and export and import of the configuration data.  
> - Data that was imported using the tool.  
> 
>   There are three log files generated by the tool that are available at the following location on the computer where you run the tool: `c:\Users\<UserName>\AppData\Roaming\Microsoft\Microsoft Dynamics 365 Configuration Migration Utility\<Version>`. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Troubleshoot configuration data migration issues using log files](/dynamics365/customer-engagement/admin/manage-configuration-data#Logfiles)  
  
  
## See also  
 [Export Unified Service Desk configuration data](../../unified-service-desk/admin/export-unified-service-desk-configuration-data.md)  
  
 [Import Unified Service Desk configuration data](../../unified-service-desk/admin/import-unified-service-desk-configuration-data.md)  