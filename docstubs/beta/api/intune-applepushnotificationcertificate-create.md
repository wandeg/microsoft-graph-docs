---
title: "Create applePushNotificationCertificate"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create applePushNotificationCertificate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new applePushNotificationCertificate object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the applePushNotificationCertificate object.

The following table shows the properties that are required when you create the applePushNotificationCertificate object.

| Property                       | Type                           | Description                                                           |
| :----------------------------- | :----------------------------- | :-------------------------------------------------------------------- |
| $(this.Properties.Name)        | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription)                                 |
| appleIdentifier                | String                         | Apple Id of the account used to create the MDM push certificate.      |
| certificate                    | String                         |                                                                       |
| certificateSerialNumber        | String                         | Certificate serial number. This property is read-only.                |
| certificateUploadFailureReason | String                         | The reason the certificate upload failed.                             |
| certificateUploadStatus        | String                         | The certificate upload status.                                        |
| expirationDateTime             | DateTimeOffset                 | The expiration date and time for Apple push notification certificate. |
| id                             | String                         | Unique Identifier for the certificate Read-only.                      |
| lastModifiedDateTime           | DateTimeOffset                 | Last modified date and time for Apple push notification certificate.  |
| topicIdentifier                | String                         | Topic Id.                                                             |

Do not supply a request body for this method.

## Response

If successful, this method returns a `201 Created` response code and a [applePushNotificationCertificate](../resources/applePushNotificationCertificate.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_applepushnotificationcertificate"
}
-->

```http
POST https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 381

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "String",
  "certificate": "String",
  "certificateSerialNumber": "String",
  "certificateUploadFailureReason": "String",
  "certificateUploadStatus": "String",
  "expirationDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset",
  "topicIdentifier": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.applePushNotificationCertificate"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "String",
  "certificate": "String",
  "certificateSerialNumber": "String",
  "certificateUploadFailureReason": "String",
  "certificateUploadStatus": "String",
  "expirationDateTime": "DateTimeOffset",
  "id": "String(identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "topicIdentifier": "String"
}
}

```