---
title: "List yammerGroupsActivityDetails"
description: "List properties and relationships of the yammerGroupsActivityDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List yammerGroupsActivityDetails

Namespace: microsoft.graph

List properties and relationships of the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) objects.

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
GET ** Collection URI for microsoft.graph.yammerGroupsActivityDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_yammergroupsactivitydetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.yammerGroupsActivityDetail not found
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
      "id": "54513b00-3b00-5451-003b-5154003b5154",
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

