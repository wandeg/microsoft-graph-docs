---
title: "appRoleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appRoleAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[checkMemberGroups](../api/approleassignment-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/approleassignment-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/approleassignment-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/approleassignment-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/approleassignment-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appRoleId|Guid|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|principalDisplayName|String|**TODO: Add Description**|
|principalId|Guid|**TODO: Add Description**|
|principalType|String|**TODO: Add Description**|
|resourceDisplayName|String|**TODO: Add Description**|
|resourceId|Guid|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "appRoleId": "Guid",
  "createdDateTime": "String (timestamp)",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
}
```

