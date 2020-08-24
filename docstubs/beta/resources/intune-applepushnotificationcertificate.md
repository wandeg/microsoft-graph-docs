---
title: "applePushNotificationCertificate resource type"
description: "Apple push notification certificate."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# applePushNotificationCertificate resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Apple push notification certificate.

## Methods

| Method                                                                                                                                                             | Return Type                                                                               | Description                                                                      |
| :----------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------- |
| [List applePushNotificationCertificate](../api/intune-applepushnotificationcertificate-list.md)                                                                    | [applePushNotificationCertificate](intune-applePushNotificationCertificate.md) collection | List properties and relationships of an applePushNotificationCertificate object. |
| [Create applePushNotificationCertificate](../api/intune-applepushnotificationcertificate-create.md)                                                                | [applePushNotificationCertificate](intune-applePushNotificationCertificate.md)            | Create a new applePushNotificationCertificate object.                            |
| [Get applePushNotificationCertificate](../api/intune-applepushnotificationcertificate-get.md)                                                                      | [applePushNotificationCertificate](intune-applePushNotificationCertificate.md)            | Read properties and relationships of an applePushNotificationCertificate object. |
| [Update applePushNotificationCertificate](../api/intune-applepushnotificationcertificate-update.md)                                                                | [applePushNotificationCertificate](intune-applePushNotificationCertificate.md)            | Update the properties of an applePushNotificationCertificate object.             |
| [Delete applePushNotificationCertificate](../api/intune-applepushnotificationcertificate-delete.md)                                                                |                                                                                           | Delete an applePushNotificationCertificate object.                               |
| [generateApplePushNotificationCertificateSigningRequest](../api/intune-applepushnotificationcertificate-generateApplePushNotificationCertificateSigningRequest.md) | String                                                                                    | Download Apple push notification certificate signing request                     |
| [downloadApplePushNotificationCertificateSigningRequest](../api/intune-applepushnotificationcertificate-downloadApplePushNotificationCertificateSigningRequest.md) | String                                                                                    | Download Apple push notification certificate signing request                     |

## Properties

| Property                       | Type           | Description                                                           |
| :----------------------------- | :------------- | :-------------------------------------------------------------------- |
| appleIdentifier                | String         | Apple Id of the account used to create the MDM push certificate.      |
| certificate                    | String         |                                                                       |
| certificateSerialNumber        | String         | Certificate serial number. This property is read-only.                |
| certificateUploadFailureReason | String         | The reason the certificate upload failed.                             |
| certificateUploadStatus        | String         | The certificate upload status.                                        |
| expirationDateTime             | DateTimeOffset | The expiration date and time for Apple push notification certificate. |
| id                             | String         | Unique Identifier for the certificate Read-only.                      |
| lastModifiedDateTime           | DateTimeOffset | Last modified date and time for Apple push notification certificate.  |
| topicIdentifier                | String         | Topic Id.                                                             |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "String",
  "certificate": "String",
  "certificateSerialNumber": "String",
  "certificateUploadFailureReason": "String",
  "certificateUploadStatus": "String",
  "expirationDateTime": "DateTimeOffset",
  "id": "String (identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "topicIdentifier": "String"
}
```