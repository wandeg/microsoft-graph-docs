---
title: "Get androidForWorkEnrollmentProfile"
description: "Read properties and relationships of the androidForWorkEnrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get androidForWorkEnrollmentProfile

Namespace: microsoft.graph

Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.

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
GET /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androidforworkenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 718

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
    "id": "b6ae9a68-9a68-b6ae-689a-aeb6689aaeb6",
    "accountId": "Account Id value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
    "tokenValue": "Token Value value",
    "tokenExpirationDateTime": "2017-01-01T00:02:47.1539709+03:00",
    "enrolledDeviceCount": 3,
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```

