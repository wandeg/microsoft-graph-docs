---
title: "mipLabel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# mipLabel resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mipLabels](../api/microsoft.directoryservices-miplabel-list.md)|[mipLabel](../resources/microsoft.directoryservices-miplabel.md) collection|Get a list of the [mipLabel](../resources/miplabel.md) objects and their properties.|
|[Get mipLabel](../api/microsoft.directoryservices-miplabel-get.md)|[mipLabel](../resources/microsoft.directoryservices-miplabel.md)|Read properties and relationships of a [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object.|
|[Create mipLabel](../api/microsoft.directoryservices-miplabel-post-miplabels.md)|[mipLabel](../resources/microsoft.directoryservices-miplabel.md)|Create a new [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object.|
|[Delete mipLabel](../api/microsoft.directoryservices-miplabel-delete.md)|None|Deletes a [mipLabel](../resources/microsoft.directoryservices-miplabel.md).|
|[Update mipLabel](../api/microsoft.directoryservices-miplabel-update.md)|[mipLabel](../resources/microsoft.directoryservices-miplabel.md)|Update the properties of a [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-miplabel-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-miplabel-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-miplabel-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-miplabel-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-miplabel-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|labelId|String|**TODO: Add Description**|
|protectGroupAction|[mipProtectGroupLabelAction](../resources/microsoft.directoryservices-mipprotectgrouplabelaction.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.mipLabel",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.mipLabel",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "labelId": "String",
  "displayName": "String",
  "protectGroupAction": {
    "@odata.type": "Microsoft.DirectoryServices.mipProtectGroupLabelAction"
  }
}
```

