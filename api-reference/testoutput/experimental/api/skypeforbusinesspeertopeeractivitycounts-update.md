---
title: "Update skypeForBusinessPeerToPeerActivityCounts"
description: "Update the properties of a skypeForBusinessPeerToPeerActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update skypeForBusinessPeerToPeerActivityCounts

Namespace: microsoft.graph

Update the properties of a [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.skypeForBusinessPeerToPeerActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|audio|Int64||
|video|Int64||
|appSharing|Int64||
|fileTransfer|Int64||
|reportRefreshDate|Date||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_skypeforbusinesspeertopeeractivitycounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.skypeForBusinessPeerToPeerActivityCounts not found
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityCounts",
  "im": 2,
  "audio": 5,
  "video": 5,
  "appSharing": 10,
  "fileTransfer": 12,
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
Content-Length: 316

{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityCounts",
  "id": "66db09d4-09d4-66db-d409-db66d409db66",
  "im": 2,
  "audio": 5,
  "video": 5,
  "appSharing": 10,
  "fileTransfer": 12,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

