---
title: "List androidDeviceOwnerEnrollmentProfiles"
description: "List properties and relationships of the androidDeviceOwnerEnrollmentProfile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List androidDeviceOwnerEnrollmentProfiles

Namespace: microsoft.graph

List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) objects.

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
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androiddeviceownerenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.androiddeviceownerenrollmentprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 910

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "id": "fb98f0ce-f0ce-fb98-cef0-98fbcef098fb",
      "accountId": "Account Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "tokenValue": "Token Value value",
      "tokenCreationDateTime": "2017-01-01T00:00:30.448772+03:00",
      "tokenExpirationDateTime": "2016-12-31T23:56:36.5597304+03:00",
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
  ]
}
```

