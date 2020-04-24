---
title: "Update shifts"
description: "Update the properties of a shifts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update shifts

Namespace: microsoft.graph

Update the properties of a shifts object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/shifts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [shift](../resources/shift.md) object.

The following table shows the properties that are required when you create the [shift](../resources/shift.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|sharedShift|[shiftItem](../resources/shiftitem.md)|**TODO: Add Description**|
|draftShift|[shiftItem](../resources/shiftitem.md)|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|schedulingGroupId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [shift](../resources/shift.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_shifts"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/shifts
Content-Type: application/json
Content-length: 605

{
  "@odata.type": "#microsoft.graph.shift",
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem",
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "theme": "String",
    "notes": "Notes value",
    "activities": [
      {
        "@odata.type": "microsoft.graph.shiftActivity",
        "isPaid": true,
        "code": "Code value"
      }
    ]
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "User Id value",
  "schedulingGroupId": "Scheduling Group Id value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.shift",
  "id": "9d7a6552-6552-9d7a-5265-7a9d52657a9d",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem",
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "theme": "String",
    "notes": "Notes value",
    "activities": [
      {
        "@odata.type": "microsoft.graph.shiftActivity",
        "isPaid": true,
        "code": "Code value"
      }
    ]
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "User Id value",
  "schedulingGroupId": "Scheduling Group Id value"
}
```

