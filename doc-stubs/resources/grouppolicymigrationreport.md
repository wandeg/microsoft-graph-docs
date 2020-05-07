---
title: "groupPolicyMigrationReport resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyMigrationReport resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[createMigrationReport](../api/grouppolicymigrationreport-createmigrationreport.md)|String|**TODO: Add Description**|
|[List groupPolicySettingMappings](../api/grouppolicymigrationreport-list-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) collection|Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property.|
|[Create groupPolicySettingMappings](../api/grouppolicymigrationreport-post-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Create a new groupPolicySettingMappings object.|
|[Delete groupPolicySettingMappings](../api/grouppolicymigrationreport-delete-grouppolicysettingmappings.md)|None|Delete a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.|
|[Update groupPolicySettingMappings](../api/grouppolicymigrationreport-update-grouppolicysettingmappings.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Update the properties of a groupPolicySettingMappings object.|
|[Get groupPolicySettingMapping](../api/grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Read the properties and relationships of a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.|
|[List unsupportedGroupPolicyExtensions](../api/grouppolicymigrationreport-list-unsupportedgrouppolicyextensions.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) collection|Get the unsupportedGroupPolicyExtensions from the unsupportedGroupPolicyExtensions navigation property.|
|[Create unsupportedGroupPolicyExtensions](../api/grouppolicymigrationreport-post-unsupportedgrouppolicyextensions.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md)|Create a new unsupportedGroupPolicyExtensions object.|
|[Delete unsupportedGroupPolicyExtensions](../api/grouppolicymigrationreport-delete-unsupportedgrouppolicyextensions.md)|None|Delete an [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.|
|[Update unsupportedGroupPolicyExtensions](../api/grouppolicymigrationreport-update-unsupportedgrouppolicyextensions.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md)|Update the properties of an unsupportedGroupPolicyExtensions object.|
|[Get unsupportedGroupPolicyExtension](../api/unsupportedgrouppolicyextension-get.md)|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md)|Read the properties and relationships of an [unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|groupPolicyCreatedDateTime|DateTimeOffset|**TODO: Add Description**|
|groupPolicyLastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|groupPolicyObjectId|Guid|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|migrationReadiness|groupPolicyMigrationReadiness|**TODO: Add Description**. Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|ouDistinguishedName|String|**TODO: Add Description**|
|supportedSettingsCount|Int32|**TODO: Add Description**|
|supportedSettingsPercent|Int32|**TODO: Add Description**|
|targetedInActiveDirectory|Boolean|**TODO: Add Description**|
|totalSettingsCount|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupPolicySettingMappings|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) collection|**TODO: Add Description**|
|unsupportedGroupPolicyExtensions|[unsupportedGroupPolicyExtension](../resources/unsupportedgrouppolicyextension.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "targetedInActiveDirectory": "Boolean",
  "totalSettingsCount": "Integer",
  "supportedSettingsCount": "Integer",
  "supportedSettingsPercent": "Integer"
}
```

