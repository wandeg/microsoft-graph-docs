---
title: "groupPolicyMigrationReport resource type"
description: "The Group Policy migration report."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyMigrationReport resource type

The Group Policy migration report.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyMigrationReport](../api/grouppolicymigrationreport-get.md)|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md)|Read properties and relationships of the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.|
|[Delete groupPolicyMigrationReport](../api/grouppolicymigrationreport-delete.md)|None|Deletes a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md).|
|[Update groupPolicyMigrationReport](../api/grouppolicymigrationreport-update.md)|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md)|Update the properties of a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.|
|[createMigrationReport](../api/grouppolicymigrationreport-createmigrationreport.md)|String||
|[List groupPolicySettingMappings](../api/grouppolicymigrationreport-list-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/groupPolicySettingMapping.md) collection|Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property.|
|[Add groupPolicySettingMappings](../api/grouppolicymigrationreport-post-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/groupPolicySettingMapping.md)|Add groupPolicySettingMappings by posting to the groupPolicySettingMappings collection.|
|[List groupPolicyMigrationReports](../api/intune-devices-devicemanagement-list-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md) collection|Get the groupPolicyMigrationReports from the groupPolicyMigrationReports navigation property.|
|[Add groupPolicyMigrationReports](../api/intune-devices-devicemanagement-post-grouppolicymigrationreports.md)|[groupPolicyMigrationReport](../resources/groupPolicyMigrationReport.md)|Add groupPolicyMigrationReports by posting to the groupPolicyMigrationReports collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was created.|
|displayName|String|The name of Group Policy Object from the GPO Xml Content|
|groupPolicyCreatedDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was created.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was last modified.|
|groupPolicyObjectId|Guid|The Group Policy Object GUID from GPO Xml content|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time at which the GroupPolicyMigrationReport was last modified.|
|migrationReadiness|Enumeration|The Intune coverage for the associated Group Policy Object file. Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|ouDistinguishedName|String|The distinguished name of the OU.|
|supportedSettingsCount|Int32|The number of Group Policy Settings supported by Intune.|
|supportedSettingsPercent|Int32|The Percentage of Group Policy Settings supported by Intune.|
|targetedInActiveDirectory|Boolean|The Targeted in AD property from GPO Xml Content|
|totalSettingsCount|Int32|The total number of Group Policy Settings from GPO file.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupPolicySettingMappings|[groupPolicySettingMapping](../resources/groupPolicySettingMapping.md) collection|A list of group policy settings to MDM/Intune mappings.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyMigrationReport",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "displayName": "String",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "groupPolicyCreatedDateTime": "String (timestamp)",
  "groupPolicyLastModifiedDateTime": "String (timestamp)",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 1024,
  "supportedSettingsCount": 1024,
  "supportedSettingsPercent": 1024
}
```

