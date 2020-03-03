---
title: "Update sharePointActivityUserCounts"
description: "Update the properties of a sharePointActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sharePointActivityUserCounts

Namespace: microsoft.graph

Update the properties of a [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.sharePointActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) object.

The following table shows the properties that are required when you create the [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|visitedPage|Int64||
|viewedOrEdited|Int64||
|synced|Int64||
|sharedInternally|Int64||
|sharedExternally|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sharepointactivityusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.sharePointActivityUserCounts not found
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.sharePointActivityUserCounts",
  "reportRefreshDate": "Date",
  "visitedPage": 11,
  "viewedOrEdited": 14,
  "synced": 6,
  "sharedInternally": 0,
  "sharedExternally": 0,
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
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.sharePointActivityUserCounts",
  "id": "b9f3b69c-b69c-b9f3-9cb6-f3b99cb6f3b9",
  "reportRefreshDate": "Date",
  "visitedPage": 11,
  "viewedOrEdited": 14,
  "synced": 6,
  "sharedInternally": 0,
  "sharedExternally": 0,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

