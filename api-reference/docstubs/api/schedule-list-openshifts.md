---
title: "List openShifts"
description: "Get the openShifts from the openShifts navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List openShifts

Namespace: microsoft.graph

Get the openShifts from the openShifts navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/openShifts
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
If successful, this method returns a `200 OK` response code and a collection of [openShift](../resources/openshift.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/openShifts
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.openshift)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.openShift",
      "id": "23f17be3-7be3-23f1-e37b-f123e37bf123",
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
      "sharedOpenShift": {
        "@odata.type": "microsoft.graph.openShiftItem",
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
        ],
        "openSlotCount": 13
      },
      "draftOpenShift": {
        "@odata.type": "microsoft.graph.openShiftItem"
      },
      "schedulingGroupId": "Scheduling Group Id value"
    }
  ]
}
```

