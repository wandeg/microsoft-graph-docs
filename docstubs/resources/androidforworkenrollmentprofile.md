---
title: "androidForWorkEnrollmentProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkEnrollmentProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[Update androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Update the properties of a [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[revokeToken](../api/androidforworkenrollmentprofile-revoketoken.md)|None||
|[createToken](../api/androidforworkenrollmentprofile-createtoken.md)|None||

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
|tokenExpirationDateTime|DateTimeOffset||
|tokenValue|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "id": "String (identifier)",
  "accountId": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  }
}
```

