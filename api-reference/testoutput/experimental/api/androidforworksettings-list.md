---
title: "List androidForWorkSettingses"
description: "List properties and relationships of the androidForWorkSettings objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List androidForWorkSettingses

List properties and relationships of the [androidForWorkSettings](../resources/androidforworksettings.md) objects.

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
GET ** Collection URI for microsoft.graph.androidForWorkSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [androidForWorkSettings](../resources/androidforworksettings.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androidforworksettings"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.androidForWorkSettings not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.androidforworksettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkSettings",
      "id": "442d411a-411a-442d-1a41-2d441a412d44",
      "bindStatus": "String",
      "lastAppSyncDateTime": "2017-01-01T00:03:22.6248676+03:00",
      "lastAppSyncStatus": "String",
      "ownerUserPrincipalName": "Owner User Principal Name value",
      "ownerOrganizationName": "Owner Organization Name value",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
      "enrollmentTarget": "String",
      "targetGroupIds": [
        "Target Group Ids value"
      ],
      "deviceOwnerManagementEnabled": true
    }
  ]
}
```

