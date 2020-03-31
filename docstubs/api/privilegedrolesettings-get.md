---
title: "Get privilegedRoleSettings"
description: "Read properties and relationships of the privilegedRoleSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get privilegedRoleSettings

Namespace: microsoft.graph

Read properties and relationships of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.

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
GET /privilegedRoles/{privilegedRolesId}/settings
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
If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}/settings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 554

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleSettings",
    "id": "a2c981f0-81f0-a2c9-f081-c9a2f081c9a2",
    "approverIds": [
      "Approver Ids value"
    ],
    "minElevationDuration": "-PT1M53.0248586S",
    "maxElavationDuration": "PT44.0712109S",
    "elevationDuration": "-PT1M51.1807882S",
    "notificationToUserOnElevation": true,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": true,
    "lastGlobalAdmin": true,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": true
  }
}
```

