---
title: "Update openShift"
description: "Update the properties of a openShift object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update openShift

Namespace: microsoft.graph

Update the properties of a [openShift](../resources/openshift.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/openShifts/{openShiftId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [openShift](../resources/openshift.md) object.

The following table shows the properties that are required when you create the [openShift](../resources/openshift.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|sharedOpenShift|[openShiftItem](../resources/openshiftitem.md)||
|draftOpenShift|[openShiftItem](../resources/openshiftitem.md)||
|schedulingGroupId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/openShifts/{openShiftId}
Content-type: application/json
Content-length: 621

{
  "@odata.type": "#microsoft.graph.openShift",
  "sharedOpenShift": {
    "@odata.type": "microsoft.graph.openShiftItem",
    "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
    "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
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
Content-Length: 1166

{
  "@odata.type": "#microsoft.graph.openShift",
  "id": "1172c444-c444-1172-44c4-721144c47211",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
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
    "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
    "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
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
```

