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
    "id": "dbd77460-7460-dbd7-6074-d7db6074d7db",
    "approverIds": [
      "Approver Ids value"
    ],
    "minElevationDuration": "-PT43.5207824S",
    "maxElavationDuration": "PT2M23.6759016S",
    "elevationDuration": "PT1M0.6100522S",
    "notificationToUserOnElevation": true,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": true,
    "lastGlobalAdmin": true,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": true
  }
}
```

