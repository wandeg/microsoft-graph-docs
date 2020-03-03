---
title: "androidForWorkEnrollmentProfile resource type"
description: "Enrollment Profile used to enroll COSU devices using Google's Cloud Management."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkEnrollmentProfile resource type


Namespace: microsoft.graph

Enrollment Profile used to enroll COSU devices using Google's Cloud Management.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidForWorkEnrollmentProfiles](../api/androidforworkenrollmentprofile-list.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) collection|List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) objects.|
|[Get androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[Create androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-create.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Create a new [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[Delete androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-delete.md)|None|Deletes a [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md).|
|[Update androidForWorkEnrollmentProfile](../api/androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Update the properties of a [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.|
|[revokeToken](../api/androidforworkenrollmentprofile-revoketoken.md)|None||
|[createToken](../api/androidforworkenrollmentprofile-createtoken.md)|None||
|[List androidForWorkEnrollmentProfiles](../api/intune-devices-devicemanagement-list-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) collection|Get the androidForWorkEnrollmentProfiles from the androidForWorkEnrollmentProfiles navigation property.|
|[Add androidForWorkEnrollmentProfiles](../api/intune-devices-devicemanagement-post-androidforworkenrollmentprofiles.md)|[androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md)|Add androidForWorkEnrollmentProfiles by posting to the androidForWorkEnrollmentProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|String|Tenant GUID the enrollment profile belongs to.|
|createdDateTime|DateTimeOffset|Date time the enrollment profile was created.|
|description|String|Description for the enrollment profile.|
|displayName|String|Display name for the enrollment profile.|
|enrolledDeviceCount|Int32|Total number of Android devices that have enrolled using this enrollment profile.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Date time the enrollment profile was last modified.|
|qrCodeContent|String|String used to generate a QR code for the token.|
|qrCodeImage|[mimeContent](../resources/intune-apps-mimecontent.md)|String used to generate a QR code for the token.|
|tokenExpirationDateTime|DateTimeOffset|Date time the most recently created token will expire.|
|tokenValue|String|Value of the most recently created token for this enrollment profile.|

## Relationships
None

## JSON Representation
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

