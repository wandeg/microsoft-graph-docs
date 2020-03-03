---
title: "resourceOperation resource type"
description: "Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC)."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# resourceOperation resource type

Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get resourceOperation](../api/resourceoperation-get.md)|[resourceOperation](../resources/resourceOperation.md)|Read properties and relationships of the [resourceOperation](../resources/resourceoperation.md) object.|
|[Delete resourceOperation](../api/resourceoperation-delete.md)|None|Deletes a [resourceOperation](../resources/resourceoperation.md).|
|[Update resourceOperation](../api/resourceoperation-update.md)|[resourceOperation](../resources/resourceOperation.md)|Update the properties of a [resourceOperation](../resources/resourceoperation.md) object.|
|[getScopesForUser](../api/resourceoperation-getscopesforuser.md)|String collection||
|[List resourceOperations](../api/intune-devices-devicemanagement-list-resourceoperations.md)|[resourceOperation](../resources/resourceOperation.md) collection|Get the resourceOperations from the resourceOperations navigation property.|
|[Add resourceOperations](../api/intune-devices-devicemanagement-post-resourceoperations.md)|[resourceOperation](../resources/resourceOperation.md)|Add resourceOperations by posting to the resourceOperations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionName|String|Type of action this operation is going to perform. The actionName should be concise and limited to as few words as possible.|
|description|String|Description of the resource operation. The description is used in mouse-over text for the operation when shown in the Azure Portal.|
|enabledForScopeValidation|Boolean|Determines whether the Permission is validated for Scopes defined per Role Assignment.|
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|String|Resource category to which this Operation belongs.|
|resourceName|String|Name of the Resource this operation is performed on.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```

