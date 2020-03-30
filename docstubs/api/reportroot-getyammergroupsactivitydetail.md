---
title: "getYammerGroupsActivityDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getYammerGroupsActivityDetail

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
GET /reports/getYammerGroupsActivityDetail
GET /print/reports/{reportRootId}/getYammerGroupsActivityDetail
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
If successful, this function returns a `200 OK` response code and a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.yammergroupsactivitydetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
      "id": "503d4af6-4af6-503d-f64a-3d50f64a3d50",
      "reportRefreshDate": "Date",
      "groupDisplayName": "Group Display Name value",
      "isDeleted": true,
      "ownerPrincipalName": "Owner Principal Name value",
      "lastActivityDate": "Date",
      "groupType": "Group Type value",
      "office365Connected": true,
      "memberCount": 11,
      "postedCount": 11,
      "readCount": 9,
      "likedCount": 10,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

