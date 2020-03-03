---
title: "Update yammerGroupsActivityGroupCounts"
description: "Update the properties of a yammerGroupsActivityGroupCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update yammerGroupsActivityGroupCounts

Update the properties of a [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.yammerGroupsActivityGroupCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [yammerGroupsActivityGroupCounts](../resources/yammerGroupsActivityGroupCounts.md) object.

The following table shows the properties that are required when you create the [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|total|Int64||
|active|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_yammergroupsactivitygroupcounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.yammerGroupsActivityGroupCounts not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

