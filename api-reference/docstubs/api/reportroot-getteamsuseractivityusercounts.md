---
title: "reportRoot: getTeamsUserActivityUserCounts"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getTeamsUserActivityUserCounts

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /reports/getTeamsUserActivityUserCounts
GET /print/reports/{reportRootId}/getTeamsUserActivityUserCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsuseractivityusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsUserActivityUserCounts",
      "id": "54f627ab-27ab-54f6-ab27-f654ab27f654",
      "reportRefreshDate": "Date",
      "reportDate": "Date",
      "teamChatMessages": 0,
      "privateChatMessages": 3,
      "calls": 5,
      "meetings": 8,
      "otherActions": 12,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

