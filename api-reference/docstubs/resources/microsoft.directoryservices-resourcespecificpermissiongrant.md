---
title: "resourceSpecificPermissionGrant resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# resourceSpecificPermissionGrant resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get resourceSpecificPermissionGrant](../api/microsoft.directoryservices-resourcespecificpermissiongrant-get.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md)|Read properties and relationships of a [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) object.|
|[Update resourceSpecificPermissionGrant](../api/microsoft.directoryservices-resourcespecificpermissiongrant-update.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md)|Update the properties of a [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-resourcespecificpermissiongrant-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-resourcespecificpermissiongrant-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-resourcespecificpermissiongrant-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-resourcespecificpermissiongrant-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-resourcespecificpermissiongrant-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientAppId|String|**TODO: Add Description**|
|clientId|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|permission|String|**TODO: Add Description**|
|permissionType|String|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
}
```

