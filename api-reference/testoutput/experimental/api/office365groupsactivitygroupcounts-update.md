---
title: "Update office365GroupsActivityGroupCounts"
description: "Update the properties of a office365GroupsActivityGroupCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update office365GroupsActivityGroupCounts

Namespace: microsoft.graph

Update the properties of a [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.office365GroupsActivityGroupCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object.

The following table shows the properties that are required when you create the [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|total|Int64||
|active|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_office365groupsactivitygroupcounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.office365GroupsActivityGroupCounts not found
Content-type: application/json
Content-length: 206

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityGroupCounts",
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
Content-Length: 255

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityGroupCounts",
  "id": "b4d2b2e3-b2e3-b4d2-e3b2-d2b4e3b2d2b4",
  "reportRefreshDate": "Date",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

