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
|Header|Value|
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
PATCH https://graph.microsoft.com/localtest/privilegedRoles/{privilegedRolesId}/settings
Content-type: application/json
Content-length: 454

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "approverIds": [
    "Approver Ids value"
  ],
  "minElevationDuration": "PT18.4564873S",
  "maxElavationDuration": "PT33.2921506S",
  "elevationDuration": "PT2M34.0794445S",
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
Content-Length: 503

{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "id": "604c132f-132f-604c-2f13-4c602f134c60",
  "approverIds": [
    "Approver Ids value"
  ],
  "minElevationDuration": "PT18.4564873S",
  "maxElavationDuration": "PT33.2921506S",
  "elevationDuration": "PT2M34.0794445S",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "mfaOnElevation": true,
  "lastGlobalAdmin": true,
  "isMfaOnElevationConfigurable": true,
  "approvalOnElevation": true
}
```

