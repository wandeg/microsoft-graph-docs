---
title: "Update sharePointSiteUsageSiteCounts"
description: "Update the properties of a sharePointSiteUsageSiteCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sharePointSiteUsageSiteCounts

Namespace: microsoft.graph

Update the properties of a [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.sharePointSiteUsageSiteCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) object.

The following table shows the properties that are required when you create the [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|siteType|String||
|total|Int64||
|active|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sharepointsiteusagesitecounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.sharePointSiteUsageSiteCounts not found
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.sharePointSiteUsageSiteCounts",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
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
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.sharePointSiteUsageSiteCounts",
  "id": "7a59cf92-cf92-7a59-92cf-597a92cf597a",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

