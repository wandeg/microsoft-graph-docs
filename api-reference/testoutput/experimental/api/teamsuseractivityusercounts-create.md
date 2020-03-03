---
title: "Create teamsUserActivityUserCounts"
description: "Create a new teamsUserActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsUserActivityUserCounts

Create a new [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.teamsUserActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the teamsUserActivityUserCounts object.

The following table shows the properties that are required when you create the teamsUserActivityUserCounts.

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
If successful, this method returns a `201 Created` response code and a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsuseractivityusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.teamsUserActivityUserCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsuseractivityusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.teamsUserActivityUserCounts",
  "id": "61d3e319-e319-61d3-19e3-d36119e3d361",
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

