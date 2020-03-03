---
title: "Create sharePointSiteUsagePages"
description: "Create a new sharePointSiteUsagePages object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sharePointSiteUsagePages

Create a new [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) object.

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
POST ** Collection URI for microsoft.graph.sharePointSiteUsagePages not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the sharePointSiteUsagePages object.

The following table shows the properties that are required when you create the sharePointSiteUsagePages.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|siteType|String||
|pageViewCount|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sharepointsiteusagepages_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.sharePointSiteUsagePages not found
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.sharePointSiteUsagePages",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "pageViewCount": 13,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharepointsiteusagepages"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.sharePointSiteUsagePages",
  "id": "8db93fe7-3fe7-8db9-e73f-b98de73fb98d",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "pageViewCount": 13,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

