---
title: "List applePushNotificationCertificates"
description: "List properties and relationships of the applePushNotificationCertificate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List applePushNotificationCertificates

Namespace: microsoft.graph

List properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.applePushNotificationCertificate not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_applepushnotificationcertificate"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.applePushNotificationCertificate not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.applepushnotificationcertificate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
      "id": "b0481aa9-1aa9-b048-a91a-48b0a91a48b0",
      "appleIdentifier": "Apple Identifier value",
      "topicIdentifier": "Topic Identifier value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "certificateUploadStatus": "Certificate Upload Status value",
      "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
      "certificate": "Certificate value"
    }
  ]
}
```

