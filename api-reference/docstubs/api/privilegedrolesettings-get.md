---
title: "Get privilegedRoleSettings"
description: "Read the properties and relationships of a privilegedRoleSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get privilegedRoleSettings

Namespace: microsoft.graph

Read the properties and relationships of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}/settings
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleSettings",
    "id": "8e3699c9-99c9-8e36-c999-368ec999368e",
    "approverIds": [
      "Approver Ids value"
    ],
    "minElevationDuration": "-PT2M37.2751317S",
    "maxElavationDuration": "PT2M57.638371S",
    "elevationDuration": "PT22.2986463S",
    "notificationToUserOnElevation": true,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": true,
    "lastGlobalAdmin": true,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": true
  }
}
```

