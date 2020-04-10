---
title: "reportRoot: getSharePointActivityUserCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSharePointActivityUserCounts

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
GET /reports/getSharePointActivityUserCounts
GET /print/reports/{reportRootId}/getSharePointActivityUserCounts
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
If successful, this function returns a `200 OK` response code and a [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sharepointactivityusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 406

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharePointActivityUserCounts",
      "id": "a282c7b7-c7b7-a282-b7c7-82a2b7c782a2",
      "reportRefreshDate": "Date",
      "visitedPage": 11,
      "viewedOrEdited": 14,
      "synced": 6,
      "sharedInternally": 0,
      "sharedExternally": 0,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

