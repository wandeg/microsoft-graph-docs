---
title: "Create oneDriveUsageAccountCounts"
description: "Create a new oneDriveUsageAccountCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create oneDriveUsageAccountCounts

Create a new [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) object.

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
POST ** Collection URI for microsoft.graph.oneDriveUsageAccountCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the oneDriveUsageAccountCounts object.

The following table shows the properties that are required when you create the oneDriveUsageAccountCounts.

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
If successful, this method returns a `201 Created` response code and a [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onedriveusageaccountcounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.oneDriveUsageAccountCounts not found
Content-type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.oneDriveUsageAccountCounts",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.onedriveusageaccountcounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 281

{
  "@odata.type": "#microsoft.graph.oneDriveUsageAccountCounts",
  "id": "88c28f65-8f65-88c2-658f-c288658fc288",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

