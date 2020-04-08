---
title: "androidDeviceOwnerEnrollmentProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidDeviceOwnerEnrollmentProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidDeviceOwnerEnrollmentProfile](../api/androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md)|Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) object.|
|[Update androidDeviceOwnerEnrollmentProfile](../api/androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md)|Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) object.|
|[revokeToken](../api/androiddeviceownerenrollmentprofile-revoketoken.md)|None||
|[createToken](../api/androiddeviceownerenrollmentprofile-createtoken.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|enrolledDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|qrCodeContent|String||
|qrCodeImage|[mimeContent](../resources/mimecontent.md)||
|roleScopeTagIds|String collection||
|tokenCreationDateTime|DateTimeOffset||
|tokenExpirationDateTime|DateTimeOffset||
|tokenValue|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "id": "String (identifier)",
  "accountId": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "roleScopeTagIds": [
    "String"
  ]
}
```

