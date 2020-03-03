---
title: "Update siteUsageStorage"
description: "Update the properties of a siteUsageStorage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update siteUsageStorage

Namespace: microsoft.graph

Update the properties of a [siteUsageStorage](../resources/siteusagestorage.md) object.

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
PATCH ** Entity URI for microsoft.graph.siteUsageStorage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [siteUsageStorage](../resources/siteusagestorage.md) object.

The following table shows the properties that are required when you create the [siteUsageStorage](../resources/siteusagestorage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|siteType|String||
|storageUsedInBytes|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [siteUsageStorage](../resources/siteusagestorage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_siteusagestorage"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.siteUsageStorage not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.siteUsageStorage",
  "id": "6c95ce11-ce11-6c95-11ce-956c11ce956c",
  "reportRefreshDate": "Date",
  "siteType": "Site Type value",
  "storageUsedInBytes": 2,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

