---
title: "List privilegedRoleSettingses"
description: "List properties and relationships of the privilegedRoleSettings objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List privilegedRoleSettingses

List properties and relationships of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) objects.

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
GET ** Collection URI for microsoft.graph.privilegedRoleSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleSettings](../resources/privilegedrolesettings.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.privilegedRoleSettings not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedrolesettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRoleSettings",
      "id": "0f5a4dcc-4dcc-0f5a-cc4d-5a0fcc4d5a0f",
      "approverIds": [
        "Approver Ids value"
      ],
      "minElevationDuration": "PT2M30.5291281S",
      "maxElavationDuration": "PT18.2951584S",
      "elevationDuration": "PT3M11.3606798S",
      "notificationToUserOnElevation": true,
      "ticketingInfoOnElevation": true,
      "mfaOnElevation": true,
      "lastGlobalAdmin": true,
      "isMfaOnElevationConfigurable": true,
      "approvalOnElevation": true
    }
  ]
}
```

