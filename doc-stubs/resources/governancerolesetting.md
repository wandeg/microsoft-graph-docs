---
title: "governanceRoleSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# governanceRoleSetting resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List governanceRoleSettings](../api/governancerolesetting-list.md)|[governanceRoleSetting](../resources/governancerolesetting.md) collection|Get a list of the [governanceRoleSetting](../resources/governancerolesetting.md) objects and their properties.|
|[Get governanceRoleSetting](../api/governancerolesetting-get.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Read the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Create governanceRoleSetting](../api/governancerolesetting-post-governancerolesettings.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Create a new [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Delete governanceRoleSetting](../api/governancerolesetting-delete.md)|None|Deletes a [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Update governanceRoleSetting](../api/governancerolesetting-update.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Update the properties of a [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[List roleDefinition](../api/governancerolesetting-list-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinition navigation property.|
|[Create roleDefinition](../api/governancerolesetting-post-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Create a new roleDefinition object.|
|[Delete roleDefinition](../api/governancerolesetting-delete-roledefinition.md)|None|Delete a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Update roleDefinition](../api/governancerolesetting-update-roledefinition.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Update the properties of a roleDefinition object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[List resource](../api/governancerolesetting-list-resource.md)|[governanceResource](../resources/governanceresource.md) collection|Get the governanceResources from the resource navigation property.|
|[Create resource](../api/governancerolesetting-post-resource.md)|[governanceResource](../resources/governanceresource.md)|Create a new resource object.|
|[Delete resource](../api/governancerolesetting-delete-resource.md)|None|Delete a [governanceResource](../resources/governanceresource.md) object.|
|[Update resource](../api/governancerolesetting-update-resource.md)|[governanceResource](../resources/governanceresource.md)|Update the properties of a resource object.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|**TODO: Add Description**|
|lastUpdatedBy|String|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceresource.md)|**TODO: Add Description**|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceRoleSetting",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": "Boolean",
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "adminMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ]
}
```

