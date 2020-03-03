---
title: "List teamsUserActivityUserDetails"
description: "List properties and relationships of the teamsUserActivityUserDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teamsUserActivityUserDetails

List properties and relationships of the [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) objects.

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
GET ** Collection URI for microsoft.graph.teamsUserActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsuseractivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.teamsUserActivityUserDetail not found
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
      "id": "5432c9ef-c9ef-5432-efc9-3254efc93254",
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

