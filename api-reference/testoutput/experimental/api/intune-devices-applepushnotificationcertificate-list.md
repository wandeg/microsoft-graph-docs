---
title: "List applePushNotificationCertificates"
description: "List properties and relationships of the applePushNotificationCertificate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List applePushNotificationCertificates

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
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.applePushNotificationCertificate not found
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
Content-Length: 597

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
      "id": "0eaa910c-910c-0eaa-0c91-aa0e0c91aa0e",
      "appleIdentifier": "Apple Identifier value",
      "topicIdentifier": "Topic Identifier value",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
      "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
      "certificateUploadStatus": "Certificate Upload Status value",
      "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
      "certificate": "Certificate value"
    }
  ]
}
```

