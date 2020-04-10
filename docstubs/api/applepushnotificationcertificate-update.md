---
title: "Update applePushNotificationCertificate"
description: "Update the properties of a applePushNotificationCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update applePushNotificationCertificate

Namespace: microsoft.graph

Update the properties of a [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appleIdentifier|String||
|topicIdentifier|String||
|lastModifiedDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|certificateUploadStatus|String||
|certificateUploadFailureReason|String||
|certificateSerialNumber|String||
|certificate|String||



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
Content-type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "e1c963a0-63a0-e1c9-a063-c9e1a063c9e1",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

