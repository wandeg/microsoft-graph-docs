---
title: "governanceRoleDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# governanceRoleDefinition resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceRoleDefinitions](../api/governanceroledefinition-list.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|Get a list of the [governanceRoleDefinition](../resources/governanceroledefinition.md) objects and their properties.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Create governanceRoleDefinition](../api/governanceroledefinition-post-governanceroledefinitions.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Create a new [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Delete governanceRoleDefinition](../api/governanceroledefinition-delete.md)|None|Deletes a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Update governanceRoleDefinition](../api/governanceroledefinition-update.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Update the properties of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[List resource](../api/governanceroledefinition-list-resource.md)|[governanceResource](../resources/governanceresource.md) collection|Get the governanceResources from the resource navigation property.|
|[Create resource](../api/governanceroledefinition-post-resource.md)|[governanceResource](../resources/governanceresource.md)|Create a new resource object.|
|[Delete resource](../api/governanceroledefinition-delete-resource.md)|None|Delete a [governanceResource](../resources/governanceresource.md) object.|
|[Update resource](../api/governanceroledefinition-update-resource.md)|[governanceResource](../resources/governanceresource.md)|Update the properties of a resource object.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.|
|[List roleSetting](../api/governanceroledefinition-list-rolesetting.md)|[governanceRoleSetting](../resources/governancerolesetting.md) collection|Get the governanceRoleSettings from the roleSetting navigation property.|
|[Create roleSetting](../api/governanceroledefinition-post-rolesetting.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Create a new roleSetting object.|
|[Delete roleSetting](../api/governanceroledefinition-delete-rolesetting.md)|None|Delete a [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Update roleSetting](../api/governanceroledefinition-update-rolesetting.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Update the properties of a roleSetting object.|
|[Get governanceRoleSetting](../api/governancerolesetting-get.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Read the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceId|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceresource.md)|**TODO: Add Description**|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "templateId": "String",
  "displayName": "String"
}
```

