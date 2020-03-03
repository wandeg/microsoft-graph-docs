---
title: "Create siteUsageStorage"
description: "Create a new siteUsageStorage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create siteUsageStorage

Create a new [siteUsageStorage](../resources/siteusagestorage.md) object.

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
POST ** Collection URI for microsoft.graph.siteUsageStorage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the siteUsageStorage object.

The following table shows the properties that are required when you create the siteUsageStorage.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|siteType|String||
|storageUsedInBytes|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [siteUsageStorage](../resources/siteusagestorage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_siteusagestorage_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.siteUsageStorage not found
Content-type: application/json
Content-length: 219

{
  "@odata.type": "#microsoft.graph.siteUsageStorage",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "storageUsedInBytes": 2,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteusagestorage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.siteUsageStorage",
  "id": "5944a1b5-a1b5-5944-b5a1-4459b5a14459",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "storageUsedInBytes": 2,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

