---
title: "reportRoot: getTeamsUserActivityUserDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getTeamsUserActivityUserDetail

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
GET /reports/getTeamsUserActivityUserDetail
GET /print/reports/{reportRootId}/getTeamsUserActivityUserDetail
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
If successful, this function returns a `200 OK` response code and a [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsuseractivityuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsUserActivityUserDetail",
      "id": "3fb88778-8778-3fb8-7887-b83f7887b83f",
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

