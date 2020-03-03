---
title: "appRoleAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# appRoleAssignment resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appRoleAssignment](../api/approleassignment-get.md)|[appRoleAssignment](../resources/appRoleAssignment.md)|Read properties and relationships of the [appRoleAssignment](../resources/approleassignment.md) object.|
|[Delete appRoleAssignment](../api/approleassignment-delete.md)|None|Deletes a [appRoleAssignment](../resources/approleassignment.md).|
|[Update appRoleAssignment](../api/approleassignment-update.md)|[appRoleAssignment](../resources/appRoleAssignment.md)|Update the properties of a [appRoleAssignment](../resources/approleassignment.md) object.|
|[List appRoleAssignments](../api/user-list-approleassignments.md)|[appRoleAssignment](../resources/appRoleAssignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Add appRoleAssignments](../api/user-post-approleassignments.md)|[appRoleAssignment](../resources/appRoleAssignment.md)|Add appRoleAssignments by posting to the appRoleAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appRoleId|Guid||
|creationTimestamp|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|principalDisplayName|String||
|principalId|Guid||
|principalType|String||
|resourceDisplayName|String||
|resourceId|Guid||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "String (identifier)",
  "appRoleId": "Guid",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
}
```

