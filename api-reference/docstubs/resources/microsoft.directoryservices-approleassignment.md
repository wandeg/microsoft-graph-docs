---
title: "appRoleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# appRoleAssignment resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List appRoleAssignments](../api/microsoft.directoryservices-approleassignment-list.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) collection|Get a list of the [appRoleAssignment](../resources/approleassignment.md) objects and their properties.|
|[Get appRoleAssignment](../api/microsoft.directoryservices-approleassignment-get.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md)|Read properties and relationships of an [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) object.|
|[Create appRoleAssignment](../api/microsoft.directoryservices-approleassignment-post-approleassignments.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md)|Create a new [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) object.|
|[Delete appRoleAssignment](../api/microsoft.directoryservices-approleassignment-delete.md)|None|Deletes an [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md).|
|[Update appRoleAssignment](../api/microsoft.directoryservices-approleassignment-update.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md)|Update the properties of a [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appRoleId|Guid|**TODO: Add Description**|
|creationTimestamp|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|principalDisplayName|String|**TODO: Add Description**|
|principalId|Guid|**TODO: Add Description**|
|principalType|String|**TODO: Add Description**|
|resourceDisplayName|String|**TODO: Add Description**|
|resourceId|Guid|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.appRoleAssignment",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.appRoleAssignment",
  "appRoleId": "Guid",
  "creationTimestamp": "String (timestamp)",
  "id": "String (identifier)",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
}
```

