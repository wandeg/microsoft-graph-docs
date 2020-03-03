---
title: "Update teamsUserActivityCounts"
description: "Update the properties of a teamsUserActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsUserActivityCounts

Update the properties of a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.teamsUserActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsUserActivityCounts](../resources/teamsUserActivityCounts.md) object.

The following table shows the properties that are required when you create the [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|reportDate|Date||
|teamChatMessages|Int64||
|privateChatMessages|Int64||
|calls|Int64||
|meetings|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsuseractivitycounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.teamsUserActivityCounts not found
Content-type: application/json
Content-length: 252

{
  "@odata.type": "#microsoft.graph.teamsUserActivityCounts",
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "teamChatMessages": 0,
  "privateChatMessages": 3,
  "calls": 5,
  "meetings": 8,
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
Content-Length: 301

{
  "@odata.type": "#microsoft.graph.teamsUserActivityCounts",
  "id": "14ab2478-2478-14ab-7824-ab147824ab14",
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "teamChatMessages": 0,
  "privateChatMessages": 3,
  "calls": 5,
  "meetings": 8,
  "reportPeriod": "Report Period value"
}
```

