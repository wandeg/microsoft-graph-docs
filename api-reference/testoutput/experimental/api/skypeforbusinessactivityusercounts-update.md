---
title: "Update skypeForBusinessActivityUserCounts"
description: "Update the properties of a skypeForBusinessActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update skypeForBusinessActivityUserCounts

Update the properties of a [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.skypeForBusinessActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessActivityUserCounts](../resources/skypeForBusinessActivityUserCounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md).

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
If successful, this method returns a `200 OK` response code and an updated [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_skypeforbusinessactivityusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.skypeForBusinessActivityUserCounts not found
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserCounts",
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
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserCounts",
  "id": "12eb6b42-6b42-12eb-426b-eb12426beb12",
  "peerToPeer": 10,
  "organized": 9,
  "participated": 12,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

