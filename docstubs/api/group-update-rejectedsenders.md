---
title: "Update rejectedSenders"
description: "Update the properties of a rejectedSenders object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update rejectedSenders

Namespace: microsoft.graph

Update the properties of a rejectedSenders object.

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
PATCH /groups/{groupsId}/rejectedSenders
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/rejectedSenders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_rejectedsenders"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/rejectedSenders
Content-Type: application/json
Content-length: 115

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "2016-12-31T23:56:33.098707+03:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "1922e6be-e6be-1922-bee6-2219bee62219",
  "deletedDateTime": "2016-12-31T23:56:33.098707+03:00"
}
```

