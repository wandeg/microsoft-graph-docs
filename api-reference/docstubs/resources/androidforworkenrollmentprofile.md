---
title: "androidForWorkEnrollmentProfile resource type"
description: "Enrollment Profile used to enroll COSU devices using Google's Cloud Management."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidForWorkEnrollmentProfile resource type


Namespace: microsoft.graph

Enrollment Profile used to enroll COSU devices using Google's Cloud Management.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Read the properties and relationships of an [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[Update androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Update the properties of an [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[revokeToken](../api/androidforworkenrollmentprofile-revoketoken.md)|None|**TODO: Add Description**|
|[createToken](../api/androidforworkenrollmentprofile-createtoken.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|String|Tenant GUID the enrollment profile belongs to.|
|createdDateTime|DateTimeOffset|Date time the enrollment profile was created.|
|description|String|Description for the enrollment profile.|
|displayName|String|Display name for the enrollment profile.|
|enrolledDeviceCount|Int32|Total number of Android devices that have enrolled using this enrollment profile.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Date time the enrollment profile was last modified.|
|qrCodeContent|String|String used to generate a QR code for the token.|
|qrCodeImage|[mimeContent](../resources/mimecontent.md)|String used to generate a QR code for the token.|
|tokenExpirationDateTime|DateTimeOffset|Date time the most recently created token will expire.|
|tokenValue|String|Value of the most recently created token for this enrollment profile.|

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

