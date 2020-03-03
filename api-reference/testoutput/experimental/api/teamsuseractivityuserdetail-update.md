---
title: "Update teamsUserActivityUserDetail"
description: "Update the properties of a teamsUserActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsUserActivityUserDetail

Update the properties of a [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.teamsUserActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsUserActivityUserDetail](../resources/teamsUserActivityUserDetail.md) object.

The following table shows the properties that are required when you create the [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|lastActivityDate|Date||
|isDeleted|Boolean||
|deletedDate|Date||
|assignedProducts|String collection||
|teamChatMessageCount|Int64||
|privateChatMessageCount|Int64||
|callCount|Int64||
|meetingCount|Int64||
|hasOtherAction|Boolean||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsuseractivityuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.teamsUserActivityUserDetail not found
Content-type: application/json
Content-length: 469

{
  "@odata.type": "#microsoft.graph.teamsUserActivityUserDetail",
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
Content-Length: 518

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
```

