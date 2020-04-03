---
title: "Update timeOffReason"
description: "Update the properties of a timeOffReason object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update timeOffReason

Namespace: microsoft.graph

Update the properties of a [timeOffReason](../resources/timeoffreason.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/timeOffReasons/{timeOffReasonId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [timeOffReason](../resources/timeoffreason.md) object.

The following table shows the properties that are required when you create the [timeOffReason](../resources/timeoffreason.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String||
|iconType|Enumeration| Possible values are: `none`, `car`, `calendar`, `running`, `plane`, `firstAid`, `doctor`, `notWorking`, `clock`, `juryDuty`, `globe`, `cup`, `phone`, `weather`, `umbrella`, `piggyBank`, `dog`, `cake`, `trafficCone`, `pin`, `sunny`, `unknownFutureValue`.|
|isActive|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [timeOffReason](../resources/timeoffreason.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_timeoffreason"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Content-length: 141

{
  "@odata.type": "#microsoft.graph.timeOffReason",
  "displayName": "Display Name value",
  "iconType": "String",
  "isActive": true
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
Content-Length: 686

{
  "@odata.type": "#microsoft.graph.timeOffReason",
  "id": "b790eb01-eb01-b790-01eb-90b701eb90b7",
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
  "iconType": "String",
  "isActive": true
}
```

