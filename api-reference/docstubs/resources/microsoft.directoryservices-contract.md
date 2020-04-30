---
title: "contract resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# contract resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List contracts](../api/microsoft.directoryservices-contract-list.md)|[contract](../resources/microsoft.directoryservices-contract.md) collection|Get a list of the [contract](../resources/contract.md) objects and their properties.|
|[Get contract](../api/microsoft.directoryservices-contract-get.md)|[contract](../resources/microsoft.directoryservices-contract.md)|Read properties and relationships of a [contract](../resources/microsoft.directoryservices-contract.md) object.|
|[Create contract](../api/microsoft.directoryservices-contract-post-contracts.md)|[contract](../resources/microsoft.directoryservices-contract.md)|Create a new [contract](../resources/microsoft.directoryservices-contract.md) object.|
|[Delete contract](../api/microsoft.directoryservices-contract-delete.md)|None|Deletes a [contract](../resources/microsoft.directoryservices-contract.md).|
|[Update contract](../api/microsoft.directoryservices-contract-update.md)|[contract](../resources/microsoft.directoryservices-contract.md)|Update the properties of a [contract](../resources/microsoft.directoryservices-contract.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-contract-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-contract-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-contract-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-contract-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-contract-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contractType|String|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|defaultDomainName|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.contract",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.contract",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String"
}
```

