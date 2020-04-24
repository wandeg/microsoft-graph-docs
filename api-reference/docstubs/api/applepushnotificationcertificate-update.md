---
title: "Update applePushNotificationCertificate"
description: "Update the properties of an applePushNotificationCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update applePushNotificationCertificate

Namespace: microsoft.graph

Update the properties of an [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appleIdentifier|String|Apple Id of the account used to create the MDM push certificate.|
|topicIdentifier|String|Topic Id.|
|lastModifiedDateTime|DateTimeOffset|Last modified date and time for Apple push notification certificate.|
|expirationDateTime|DateTimeOffset|The expiration date and time for Apple push notification certificate.|
|certificateUploadStatus|String|The certificate upload status.|
|certificateUploadFailureReason|String|The reason the certificate upload failed.|
|certificateSerialNumber|String|Certificate serial number. This property is read-only.|
|certificate|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_applepushnotificationcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-Type: application/json
Content-length: 480

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "0387d9a9-d9a9-0387-a9d9-8703a9d98703",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

