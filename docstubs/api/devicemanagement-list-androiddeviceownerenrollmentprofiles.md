---
title: "List androidDeviceOwnerEnrollmentProfiles"
description: "Get the androidDeviceOwnerEnrollmentProfiles from the androidDeviceOwnerEnrollmentProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List androidDeviceOwnerEnrollmentProfiles

Namespace: microsoft.graph

Get the androidDeviceOwnerEnrollmentProfiles from the androidDeviceOwnerEnrollmentProfiles navigation property.

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
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/androiddeviceownerenrollmentprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androiddeviceownerenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
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
Content-Length: 912

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "id": "12c83fca-3fca-12c8-ca3f-c812ca3fc812",
      "accountId": "Account Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
      "tokenValue": "Token Value value",
      "tokenCreationDateTime": "2016-12-31T23:58:21.8950946+03:00",
      "tokenExpirationDateTime": "2016-12-31T23:59:06.9056119+03:00",
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

