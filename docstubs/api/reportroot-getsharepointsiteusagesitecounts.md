---
title: "getSharePointSiteUsageSiteCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSharePointSiteUsageSiteCounts

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
GET /reports/getSharePointSiteUsageSiteCounts
GET /print/reports/{reportRootId}/getSharePointSiteUsageSiteCounts
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
If successful, this function returns a `200 OK` response code and a [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sharepointsiteusagesitecounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharePointSiteUsageSiteCounts",
      "id": "b5e5232c-232c-b5e5-2c23-e5b52c23e5b5",
      "reportRefreshDate": "Date",
      "siteType": "Site Type value",
      "total": 5,
      "active": 6,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

