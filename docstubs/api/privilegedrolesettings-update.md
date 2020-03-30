---
title: "Update privilegedRoleSettings"
description: "Update the properties of a privilegedRoleSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedRoleSettings

Namespace: microsoft.graph

Update the properties of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.

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
PATCH /privilegedRoles/{privilegedRolesId}/settings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.

The following table shows the properties that are required when you create the [privilegedRoleSettings](../resources/privilegedrolesettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|approverIds|String collection||
|minElevationDuration|Duration||
|maxElavationDuration|Duration||
|elevationDuration|Duration||
|notificationToUserOnElevation|Boolean||
|ticketingInfoOnElevation|Boolean||
|mfaOnElevation|Boolean||
|lastGlobalAdmin|Boolean||
|isMfaOnElevationConfigurable|Boolean||
|approvalOnElevation|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedrolesettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}/settings
Content-type: application/json
Content-length: 458

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "approverIds": [
    "Approver Ids value"
  ],
  "minElevationDuration": "PT3M25.9067524S",
  "maxElavationDuration": "PT2M6.9915451S",
  "elevationDuration": "-PT2M57.4644889S",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "mfaOnElevation": true,
  "lastGlobalAdmin": true,
  "isMfaOnElevationConfigurable": true,
  "approvalOnElevation": true
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
Content-Length: 507

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "id": "e12c6ee5-6ee5-e12c-e56e-2ce1e56e2ce1",
  "approverIds": [
    "Approver Ids value"
  ],
  "minElevationDuration": "PT3M25.9067524S",
  "maxElavationDuration": "PT2M6.9915451S",
  "elevationDuration": "-PT2M57.4644889S",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "mfaOnElevation": true,
  "lastGlobalAdmin": true,
  "isMfaOnElevationConfigurable": true,
  "approvalOnElevation": true
}
```

