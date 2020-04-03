---
title: "Get androidDeviceOwnerEnrollmentProfile"
description: "Read properties and relationships of the androidDeviceOwnerEnrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get androidDeviceOwnerEnrollmentProfile

Namespace: microsoft.graph

Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) object.

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
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
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
If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androiddeviceownerenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 858

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
    "id": "1fccfb15-fb15-1fcc-15fb-cc1f15fbcc1f",
    "accountId": "Account Id value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "tokenValue": "Token Value value",
    "tokenCreationDateTime": "2016-12-31T23:56:43.5678309+00:00",
    "tokenExpirationDateTime": "2017-01-01T00:00:36.9582138+00:00",
    "enrolledDeviceCount": 3,
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```

