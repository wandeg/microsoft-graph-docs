---
title: "Update yammerGroupsActivityCounts"
description: "Update the properties of a yammerGroupsActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update yammerGroupsActivityCounts

Namespace: microsoft.graph

Update the properties of a [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.yammerGroupsActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object.

The following table shows the properties that are required when you create the [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|liked|Int64||
|posted|Int64||
|read|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_yammergroupsactivitycounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.yammerGroupsActivityCounts not found
Content-type: application/json
Content-length: 212

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityCounts",
  "reportRefreshDate": "Date",
  "liked": 5,
  "posted": 6,
  "read": 4,
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
Content-Length: 261

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityCounts",
  "id": "64d35fa4-5fa4-64d3-a45f-d364a45fd364",
  "reportRefreshDate": "Date",
  "liked": 5,
  "posted": 6,
  "read": 4,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

