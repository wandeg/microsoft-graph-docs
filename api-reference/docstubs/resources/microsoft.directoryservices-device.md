---
title: "device resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# device resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List devices](../api/microsoft.directoryservices-device-list.md)|[device](../resources/microsoft.directoryservices-device.md) collection|Get a list of the [device](../resources/device.md) objects and their properties.|
|[Get device](../api/microsoft.directoryservices-device-get.md)|[device](../resources/microsoft.directoryservices-device.md)|Read properties and relationships of a [device](../resources/microsoft.directoryservices-device.md) object.|
|[Create device](../api/microsoft.directoryservices-device-post-devices.md)|[device](../resources/microsoft.directoryservices-device.md)|Create a new [device](../resources/microsoft.directoryservices-device.md) object.|
|[Delete device](../api/microsoft.directoryservices-device-delete.md)|None|Deletes a [device](../resources/microsoft.directoryservices-device.md).|
|[Update device](../api/microsoft.directoryservices-device-update.md)|[device](../resources/microsoft.directoryservices-device.md)|Update the properties of a [device](../resources/microsoft.directoryservices-device.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-device-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-device-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-device-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-device-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-device-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[List memberOf](../api/microsoft.directoryservices-device-list-memberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/microsoft.directoryservices-device-post-memberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/microsoft.directoryservices-device-delete-memberof.md)|None|Remove a memberOf object.|
|[List registeredOwners](../api/microsoft.directoryservices-device-list-registeredowners.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the registeredOwners navigation property.|
|[Add registeredOwners](../api/microsoft.directoryservices-device-post-registeredowners.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add registeredOwners by posting to the registeredOwners collection.|
|[Remove registeredOwners](../api/microsoft.directoryservices-device-delete-registeredowners.md)|None|Remove a registeredOwners object.|
|[List registeredUsers](../api/microsoft.directoryservices-device-list-registeredusers.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the registeredUsers navigation property.|
|[Add registeredUsers](../api/microsoft.directoryservices-device-post-registeredusers.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add registeredUsers by posting to the registeredUsers collection.|
|[Remove registeredUsers](../api/microsoft.directoryservices-device-delete-registeredusers.md)|None|Remove a registeredUsers object.|
|[List transitiveMemberOf](../api/microsoft.directoryservices-device-list-transitivememberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/microsoft.directoryservices-device-post-transitivememberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/microsoft.directoryservices-device-delete-transitivememberof.md)|None|Remove a transitiveMemberOf object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|alternativeSecurityIds|[alternativeSecurityId](../resources/microsoft.directoryservices-alternativesecurityid.md) collection|**TODO: Add Description**|
|approximateLastSignInDateTime|DateTimeOffset|**TODO: Add Description**|
|complianceExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deviceId|String|**TODO: Add Description**|
|deviceMetadata|String|**TODO: Add Description**|
|deviceVersion|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|isCompliant|Boolean|**TODO: Add Description**|
|isManaged|Boolean|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|operatingSystem|String|**TODO: Add Description**|
|operatingSystemVersion|String|**TODO: Add Description**|
|physicalIds|String collection|**TODO: Add Description**|
|profileType|String|**TODO: Add Description**|
|systemLabels|String collection|**TODO: Add Description**|
|trustType|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|memberOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|registeredOwners|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|registeredUsers|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.device",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.device",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "Microsoft.DirectoryServices.alternativeSecurityId",
      "type": 1024,
      "identityProvider": "String",
      "key": "binary"
    }
  ],
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "deviceId": "String",
  "deviceMetadata": "String",
  "deviceVersion": 1024,
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "String",
  "operatingSystemVersion": "String",
  "physicalIds": [
    "String"
  ],
  "profileType": "String",
  "systemLabels": [
    "String"
  ],
  "trustType": "String"
}
```

