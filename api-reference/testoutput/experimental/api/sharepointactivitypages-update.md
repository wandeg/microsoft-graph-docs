---
title: "Update sharePointActivityPages"
description: "Update the properties of a sharePointActivityPages object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sharePointActivityPages

Namespace: microsoft.graph

Update the properties of a [sharePointActivityPages](../resources/sharepointactivitypages.md) object.

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
PATCH ** Entity URI for microsoft.graph.sharePointActivityPages not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [sharePointActivityPages](../resources/sharepointactivitypages.md) object.

The following table shows the properties that are required when you create the [sharePointActivityPages](../resources/sharepointactivitypages.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|visitedPageCount|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [sharePointActivityPages](../resources/sharepointactivitypages.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sharepointactivitypages"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.sharePointActivityPages not found
Content-type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.sharePointActivityPages",
  "reportRefreshDate": "Date",
  "visitedPageCount": 0,
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
Content-Length: 239

{
  "@odata.type": "#microsoft.graph.sharePointActivityPages",
  "id": "cd805508-5508-cd80-0855-80cd085580cd",
  "reportRefreshDate": "Date",
  "visitedPageCount": 0,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

