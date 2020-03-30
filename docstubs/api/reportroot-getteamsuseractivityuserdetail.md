---
title: "getTeamsUserActivityUserDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getTeamsUserActivityUserDetail

Namespace: microsoft.graph



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
GET /reports/getTeamsUserActivityUserDetail
GET /print/reports/{reportRootId}/getTeamsUserActivityUserDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsuseractivityuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsUserActivityUserDetail",
      "id": "f5575c58-5c58-f557-585c-57f5585c57f5",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "lastActivityDate": "Date",
      "isDeleted": true,
      "deletedDate": "Date",
      "assignedProducts": [
        "Assigned Products value"
      ],
      "teamChatMessageCount": 4,
      "privateChatMessageCount": 7,
      "callCount": 9,
      "meetingCount": 12,
      "hasOtherAction": true,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

