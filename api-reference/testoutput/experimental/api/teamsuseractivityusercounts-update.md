---
title: "Update teamsUserActivityUserCounts"
description: "Update the properties of a teamsUserActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsUserActivityUserCounts

Namespace: microsoft.graph

Update the properties of a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.teamsUserActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object.

The following table shows the properties that are required when you create the [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|reportDate|Date||
|teamChatMessages|Int64||
|privateChatMessages|Int64||
|calls|Int64||
|meetings|Int64||
|otherActions|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsuseractivityusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.teamsUserActivityUserCounts not found
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.teamsUserActivityUserCounts",
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "teamChatMessages": 0,
  "privateChatMessages": 3,
  "calls": 5,
  "meetings": 8,
  "otherActions": 12,
  "reportPeriod": "Report Period value"
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
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.teamsUserActivityUserCounts",
  "id": "2d3e27c2-27c2-2d3e-c227-3e2dc2273e2d",
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "teamChatMessages": 0,
  "privateChatMessages": 3,
  "calls": 5,
  "meetings": 8,
  "otherActions": 12,
  "reportPeriod": "Report Period value"
}
```

