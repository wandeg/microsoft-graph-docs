---
title: "governanceRoleDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governanceRoleDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceRoleDefinitions](../api/governanceroledefinition-list.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|List properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) objects.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Create governanceRoleDefinition](../api/governanceroledefinition-post-governanceroledefinitions.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Create a new [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Delete governanceRoleDefinition](../api/governanceroledefinition-delete.md)|None|Deletes a [governanceRoleDefinition](../resources/governanceroledefinition.md).|
|[Update governanceRoleDefinition](../api/governanceroledefinition-update.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Update the properties of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[Get governanceRoleSetting](../api/governancerolesetting-get.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Read properties and relationships of the [governanceRoleSetting](../resources/governancerolesetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceId|String||
|templateId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceresource.md)||
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)||

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

