---
title: "getYammerGroupsActivityGroupCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getYammerGroupsActivityGroupCounts

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
GET /reports/getYammerGroupsActivityGroupCounts
GET /print/reports/{reportRootId}/getYammerGroupsActivityGroupCounts
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
If successful, this function returns a `200 OK` response code and a [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.yammergroupsactivitygroupcounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.yammerGroupsActivityGroupCounts",
      "id": "2c9c9485-9485-2c9c-8594-9c2c85949c2c",
      "reportRefreshDate": "Date",
      "total": 5,
      "active": 6,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

