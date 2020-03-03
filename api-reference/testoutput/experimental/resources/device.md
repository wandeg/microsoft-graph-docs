---
title: "device resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# device resource type

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get device](../api/device-get.md)|[device](../resources/device.md)|Read properties and relationships of the [device](../resources/device.md) object.|
|[Delete device](../api/device-delete.md)|None|Deletes a [device](../resources/device.md).|
|[Update device](../api/device-update.md)|[device](../resources/device.md)|Update the properties of a [device](../resources/device.md) object.|
|[checkMemberGroups](../api/device-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/device-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/device-getmembergroups.md)|String collection||
|[getMemberObjects](../api/device-getmemberobjects.md)|String collection||
|[restore](../api/device-restore.md)|[directoryObject](../resources/directoryObject.md)||
|[List memberOf](../api/device-list-memberof.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Create memberOf](../api/device-post-memberof.md)|[directoryObject](../resources/directoryObject.md)|Create memberOf by posting to the memberOf collection.|
|[List registeredOwners](../api/device-list-registeredowners.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the registeredOwners navigation property.|
|[Create registeredOwners](../api/device-post-registeredowners.md)|[directoryObject](../resources/directoryObject.md)|Create registeredOwners by posting to the registeredOwners collection.|
|[List registeredUsers](../api/device-list-registeredusers.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the registeredUsers navigation property.|
|[Create registeredUsers](../api/device-post-registeredusers.md)|[directoryObject](../resources/directoryObject.md)|Create registeredUsers by posting to the registeredUsers collection.|
|[List transitiveMemberOf](../api/device-list-transitivememberof.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Create transitiveMemberOf](../api/device-post-transitivememberof.md)|[directoryObject](../resources/directoryObject.md)|Create transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[List extensions](../api/device-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/device-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List commands](../api/device-list-commands.md)|[command](../resources/command.md) collection|Get the commands from the commands navigation property.|
|[Add commands](../api/device-post-commands.md)|[command](../resources/command.md)|Add commands by posting to the commands collection.|
|[List devices](../api/user-list-devices.md)|[device](../resources/device.md) collection|Get the devices from the devices navigation property.|
|[Add devices](../api/user-post-devices.md)|[device](../resources/device.md)|Add devices by posting to the devices collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean||
|alternativeSecurityIds|[alternativeSecurityId](../resources/alternativeSecurityId.md) collection||
|approximateLastSignInDateTime|DateTimeOffset||
|complianceExpirationDateTime|DateTimeOffset||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|deviceId|String||
|deviceMetadata|String||
|deviceVersion|Int32||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isCompliant|Boolean||
|isManaged|Boolean||
|Kind|String||
|Manufacturer|String||
|Model|String||
|Name|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesSyncEnabled|Boolean||
|operatingSystem|String||
|operatingSystemVersion|String||
|physicalIds|String collection||
|Platform|String||
|profileType|String||
|Status|String||
|systemLabels|String collection||
|trustType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|commands|[command](../resources/command.md) collection||
|extensions|[extension](../resources/extension.md) collection||
|memberOf|[directoryObject](../resources/directoryObject.md) collection||
|registeredOwners|[directoryObject](../resources/directoryObject.md) collection||
|registeredUsers|[directoryObject](../resources/directoryObject.md) collection||
|transitiveMemberOf|[directoryObject](../resources/directoryObject.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.device",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
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
  "trustType": "String",
  "Name": "String",
  "Manufacturer": "String",
  "Model": "String",
  "Kind": "String",
  "Status": "String",
  "Platform": "String"
}
```

