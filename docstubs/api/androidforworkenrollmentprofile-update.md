---
title: "Update androidForWorkEnrollmentProfile"
description: "Update the properties of a androidForWorkEnrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update androidForWorkEnrollmentProfile

Namespace: microsoft.graph

Update the properties of a [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.

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
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.

The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accountId|String||
|displayName|String||
|description|String||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|tokenValue|String||
|tokenExpirationDateTime|DateTimeOffset||
|enrolledDeviceCount|Int32||
|qrCodeContent|String||
|qrCodeImage|[mimeContent](../resources/mimecontent.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_androidforworkenrollmentprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2017-01-01T00:00:36.9582138+00:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "id": "014714e1-14e1-0147-e114-4701e1144701",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2017-01-01T00:00:36.9582138+00:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

