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
Content-length: 457

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "approverIds": [
    "Approver Ids value"
  ],
  "minElevationDuration": "-PT3M29.5304397S",
  "maxElavationDuration": "PT2M4.0259314S",
  "elevationDuration": "PT2M2.5979593S",
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
Content-Length: 506

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "id": "e6e085d0-85d0-e6e0-d085-e0e6d085e0e6",
  "approverIds": [
    "Approver Ids value"
  ],
  "minElevationDuration": "-PT3M29.5304397S",
  "maxElavationDuration": "PT2M4.0259314S",
  "elevationDuration": "PT2M2.5979593S",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "mfaOnElevation": true,
  "lastGlobalAdmin": true,
  "isMfaOnElevationConfigurable": true,
  "approvalOnElevation": true
}
```

