---
title: "Create yammerGroupsActivityCounts"
description: "Create a new yammerGroupsActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create yammerGroupsActivityCounts

Namespace: microsoft.graph

Create a new [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object.

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
POST ** Collection URI for microsoft.graph.yammerGroupsActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_yammergroupsactivitycounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.yammerGroupsActivityCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.yammergroupsactivitycounts"
}
-->
``` http
HTTP/1.1 201 Created
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

