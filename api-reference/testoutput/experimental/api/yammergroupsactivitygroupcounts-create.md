---
title: "Create yammerGroupsActivityGroupCounts"
description: "Create a new yammerGroupsActivityGroupCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create yammerGroupsActivityGroupCounts

Create a new [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object.

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
POST ** Collection URI for microsoft.graph.yammerGroupsActivityGroupCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the yammerGroupsActivityGroupCounts object.

The following table shows the properties that are required when you create the yammerGroupsActivityGroupCounts.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|total|Int64||
|active|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_yammergroupsactivitygroupcounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.yammerGroupsActivityGroupCounts not found
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityGroupCounts",
  "reportRefreshDate": "Date",
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
  "@odata.type": "microsoft.graph.yammergroupsactivitygroupcounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityGroupCounts",
  "id": "db7af787-f787-db7a-87f7-7adb87f77adb",
  "reportRefreshDate": "Date",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

