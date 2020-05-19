---
title: "contract resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# contract resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[checkMemberGroups](../api/contract-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/contract-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/contract-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/contract-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/contract-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contractType|String|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|defaultDomainName|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contract",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contract",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String"
}
```

