---
title: "List calendarPermissions"
description: "Get the calendarPermissions from the calendarPermissions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List calendarPermissions

Namespace: microsoft.graph

Get the calendarPermissions from the calendarPermissions navigation property.

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
GET /users/{usersId}/messages/{messageId}/event/calendar/calendarPermissions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [calendarPermission](../resources/calendarpermission.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/messages/{messageId}/event/calendar/calendarPermissions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.calendarpermission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.calendarPermission",
      "id": "2afcbc1d-bc1d-2afc-1dbc-fc2a1dbcfc2a",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress"
      },
      "isRemovable": "Boolean",
      "isInsideOrganization": "Boolean",
      "role": "String",
      "allowedRoles": [
        "String"
      ]
    }
  ]
}
```

