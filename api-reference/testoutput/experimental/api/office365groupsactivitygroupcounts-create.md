---
title: "Create office365GroupsActivityGroupCounts"
description: "Create a new office365GroupsActivityGroupCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365GroupsActivityGroupCounts

Create a new [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365GroupsActivityGroupCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the office365GroupsActivityGroupCounts object.

The following table shows the properties that are required when you create the office365GroupsActivityGroupCounts.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|total|Int64||
|active|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365groupsactivitygroupcounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.office365GroupsActivityGroupCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.office365groupsactivitygroupcounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 255

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityGroupCounts",
  "id": "6b1c755d-755d-6b1c-5d75-1c6b5d751c6b",
  "reportRefreshDate": "Date",
  "total": 5,
  "active": 6,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

