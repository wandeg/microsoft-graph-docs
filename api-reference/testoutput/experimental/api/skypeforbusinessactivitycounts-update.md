---
title: "Update skypeForBusinessActivityCounts"
description: "Update the properties of a skypeForBusinessActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update skypeForBusinessActivityCounts

Namespace: microsoft.graph

Update the properties of a [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.skypeForBusinessActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|peerToPeer|Int64||
|organized|Int64||
|participated|Int64||
|reportRefreshDate|Date||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_skypeforbusinessactivitycounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.skypeForBusinessActivityCounts not found
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityCounts",
  "peerToPeer": 10,
  "organized": 9,
  "participated": 12,
  "reportRefreshDate": "Date",
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
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityCounts",
  "id": "51aa4c86-4c86-51aa-864c-aa51864caa51",
  "peerToPeer": 10,
  "organized": 9,
  "participated": 12,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

