---
title: "Create skypeForBusinessActivityCounts"
description: "Create a new skypeForBusinessActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create skypeForBusinessActivityCounts

Namespace: microsoft.graph

Create a new [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object.

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
POST ** Collection URI for microsoft.graph.skypeForBusinessActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_skypeforbusinessactivitycounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.skypeForBusinessActivityCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeforbusinessactivitycounts"
}
-->
``` http
HTTP/1.1 201 Created
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

