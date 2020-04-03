---
title: "Get schedulingGroup"
description: "Read properties and relationships of the schedulingGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get schedulingGroup

Namespace: microsoft.graph

Read properties and relationships of the [schedulingGroup](../resources/schedulinggroup.md) object.

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
GET /me/joinedGroups/{groupId}/team/schedule/schedulingGroups/{schedulingGroupId}
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
If successful, this method returns a `200 OK` response code and [schedulingGroup](../resources/schedulinggroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schedulinggroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/schedulingGroups/{schedulingGroupId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 772

{
  "value": {
    "@odata.type": "#microsoft.graph.schedulingGroup",
    "id": "ea8cac8e-ac8e-ea8c-8eac-8cea8eac8cea",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "displayName": "Display Name value",
    "isActive": true,
    "userIds": [
      "User Ids value"
    ]
  }
}
```

