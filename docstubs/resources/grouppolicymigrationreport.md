---
title: "groupPolicyMigrationReport resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyMigrationReport resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyMigrationReport](../api/grouppolicymigrationreport-get.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md)|Read properties and relationships of the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.|
|[Update groupPolicyMigrationReport](../api/grouppolicymigrationreport-update.md)|[groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md)|Update the properties of a [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.|
|[createMigrationReport](../api/grouppolicymigrationreport-createmigrationreport.md)|String||
|[List groupPolicySettingMappings](../api/grouppolicymigrationreport-list-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) collection|Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property.|
|[Add groupPolicySettingMappings](../api/grouppolicymigrationreport-post-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Add groupPolicySettingMappings by posting to the groupPolicySettingMappings collection.|
|[List unsupportedGroupPolicyExtensions](../api/grouppolicymigrationreport-list-unsupportedgrouppolicyextensions.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) collection|Get the unsupportedGroupPolicyExtensions from the unsupportedGroupPolicyExtensions navigation property.|
|[Add unsupportedGroupPolicyExtensions](../api/grouppolicymigrationreport-post-unsupportedgrouppolicyextensions.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md)|Add unsupportedGroupPolicyExtensions by posting to the unsupportedGroupPolicyExtensions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|displayName|String||
|groupPolicyCreatedDateTime|DateTimeOffset||
|groupPolicyLastModifiedDateTime|DateTimeOffset||
|groupPolicyObjectId|Guid||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|migrationReadiness|Enumeration| Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|ouDistinguishedName|String||
|supportedSettingsCount|Int32||
|supportedSettingsPercent|Int32||
|targetedInActiveDirectory|Boolean||
|totalSettingsCount|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupPolicySettingMappings|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) collection||
|unsupportedGroupPolicyExtensions|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) collection||

## JSON representation
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

