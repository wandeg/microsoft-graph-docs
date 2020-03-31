---
title: "Update schedulingGroup"
description: "Update the properties of a schedulingGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update schedulingGroup

Namespace: microsoft.graph

Update the properties of a [schedulingGroup](../resources/schedulinggroup.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/schedulingGroups/{schedulingGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [schedulingGroup](../resources/schedulinggroup.md) object.

The following table shows the properties that are required when you create the [schedulingGroup](../resources/schedulinggroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String||
|isActive|Boolean||
|userIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [schedulingGroup](../resources/schedulinggroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_schedulinggroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/schedulingGroups/{schedulingGroupId}
Content-type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.schedulingGroup",
  "displayName": "Display Name value",
  "isActive": true,
  "userIds": [
    "User Ids value"
  ]
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
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.schedulingGroup",
  "id": "bcb0dc16-dc16-bcb0-16dc-b0bc16dcb0bc",
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
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
```

