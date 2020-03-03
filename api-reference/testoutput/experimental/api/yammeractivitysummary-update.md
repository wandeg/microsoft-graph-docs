---
title: "Update yammerActivitySummary"
description: "Update the properties of a yammerActivitySummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update yammerActivitySummary

Update the properties of a [yammerActivitySummary](../resources/yammeractivitysummary.md) object.

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
PATCH ** Entity URI for microsoft.graph.yammerActivitySummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [yammerActivitySummary](../resources/yammerActivitySummary.md) object.

The following table shows the properties that are required when you create the [yammerActivitySummary](../resources/yammeractivitysummary.md).

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
If successful, this method returns a `200 OK` response code and an updated [yammerActivitySummary](../resources/yammeractivitysummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_yammeractivitysummary"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.yammerActivitySummary not found
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.yammerActivitySummary",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "@odata.type": "#microsoft.graph.yammerActivitySummary",
  "id": "1d1f1b64-1b64-1d1f-641b-1f1d641b1f1d",
  "reportRefreshDate": "Date",
  "liked": 5,
  "posted": 6,
  "read": 4,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

