---
title: "applePushNotificationCertificate resource type"
description: "Apple push notification certificate."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# applePushNotificationCertificate resource type

Apple push notification certificate.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List applePushNotificationCertificates](../api/intune-devices-applepushnotificationcertificate-list.md)|[applePushNotificationCertificate](../resources/intune-devices-applePushNotificationCertificate.md) collection|List properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) objects.|
|[Get applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applePushNotificationCertificate.md)|Read properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Create applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-create.md)|[applePushNotificationCertificate](../resources/intune-devices-applePushNotificationCertificate.md)|Create a new [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Delete applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-delete.md)|None|Deletes a [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md).|
|[Update applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applePushNotificationCertificate.md)|Update the properties of a [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[downloadApplePushNotificationCertificateSigningRequest](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdentifier|String|Apple Id of the account used to create the MDM push certificate.|
|certificate|String||
|certificateUploadFailureReason|String|The reason the certificate upload failed.|
|certificateUploadStatus|String|The certificate upload status.|
|expirationDateTime|DateTimeOffset|The expiration date and time for Apple push notification certificate.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified date and time for Apple push notification certificate.|
|topicIdentifier|String|Topic Id.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificate": "String"
}
```

