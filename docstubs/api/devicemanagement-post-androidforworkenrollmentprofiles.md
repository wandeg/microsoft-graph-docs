---
title: "Add androidForWorkEnrollmentProfiles"
description: "Add androidForWorkEnrollmentProfiles by posting to the androidForWorkEnrollmentProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add androidForWorkEnrollmentProfiles

Namespace: microsoft.graph

Add androidForWorkEnrollmentProfiles by posting to the androidForWorkEnrollmentProfiles collection.

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
POST /deviceManagement/androidForWorkEnrollmentProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_androidforworkenrollmentprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2017-01-01T00:01:02.750201+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.androidforworkenrollmentprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "id": "a0b489c8-89c8-a0b4-c889-b4a0c889b4a0",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2017-01-01T00:01:02.750201+03:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

