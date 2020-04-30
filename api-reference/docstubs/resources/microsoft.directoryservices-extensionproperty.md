---
title: "extensionProperty resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# extensionProperty resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get extensionProperty](../api/microsoft.directoryservices-extensionproperty-get.md)|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md)|Read properties and relationships of an [extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) object.|
|[Update extensionProperty](../api/microsoft.directoryservices-extensionproperty-update.md)|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md)|Update the properties of a [extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-extensionproperty-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-extensionproperty-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-extensionproperty-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-extensionproperty-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-extensionproperty-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String|**TODO: Add Description**|
|dataType|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|isSyncedFromOnPremises|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|targetObjects|String collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.extensionProperty",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.extensionProperty",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "String"
  ]
}
```

