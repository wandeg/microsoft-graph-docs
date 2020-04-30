---
title: "scopedRoleMembership resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# scopedRoleMembership resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List scopedRoleMemberships](../api/microsoft.directoryservices-scopedrolemembership-list.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) collection|Get a list of the [scopedRoleMembership](../resources/scopedrolemembership.md) objects and their properties.|
|[Get scopedRoleMembership](../api/microsoft.directoryservices-scopedrolemembership-get.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Read properties and relationships of a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.|
|[Create scopedRoleMembership](../api/microsoft.directoryservices-scopedrolemembership-post-scopedrolememberships.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Create a new [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.|
|[Delete scopedRoleMembership](../api/microsoft.directoryservices-scopedrolemembership-delete.md)|None|Deletes a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md).|
|[Update scopedRoleMembership](../api/microsoft.directoryservices-scopedrolemembership-update.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Update the properties of a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|administrativeUnitId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|roleMemberInfo|[identity](../resources/microsoft.directoryservices-identity.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.scopedRoleMembership",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.scopedRoleMembership",
  "id": "String (identifier)",
  "roleId": "String",
  "administrativeUnitId": "String",
  "roleMemberInfo": {
    "@odata.type": "Microsoft.DirectoryServices.identity"
  }
}
```

