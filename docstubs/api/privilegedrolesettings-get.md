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
Content-Length: 552

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleSettings",
    "id": "3bf9d59b-d59b-3bf9-9bd5-f93b9bd5f93b",
    "approverIds": [
      "Approver Ids value"
    ],
    "minElevationDuration": "PT2M35.9478986S",
    "maxElavationDuration": "PT2M5.1604962S",
    "elevationDuration": "-PT45.4823994S",
    "notificationToUserOnElevation": true,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": true,
    "lastGlobalAdmin": true,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": true
  }
}
```

