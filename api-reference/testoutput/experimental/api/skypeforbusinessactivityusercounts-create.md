---
title: "Create skypeForBusinessActivityUserCounts"
description: "Create a new skypeForBusinessActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create skypeForBusinessActivityUserCounts

Namespace: microsoft.graph

Create a new [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.skypeForBusinessActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object.

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
If successful, this method returns a `201 Created` response code and a [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_skypeforbusinessactivityusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.skypeForBusinessActivityUserCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeforbusinessactivityusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserCounts",
  "id": "697a5efe-5efe-697a-fe5e-7a69fe5e7a69",
  "peerToPeer": 10,
  "organized": 9,
  "participated": 12,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

