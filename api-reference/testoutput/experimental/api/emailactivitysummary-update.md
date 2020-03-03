---
title: "Update emailActivitySummary"
description: "Update the properties of a emailActivitySummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update emailActivitySummary

Namespace: microsoft.graph

Update the properties of a [emailActivitySummary](../resources/emailactivitysummary.md) object.

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
PATCH ** Entity URI for microsoft.graph.emailActivitySummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [emailActivitySummary](../resources/emailactivitysummary.md) object.

The following table shows the properties that are required when you create the [emailActivitySummary](../resources/emailactivitysummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|send|Int64||
|receive|Int64||
|read|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [emailActivitySummary](../resources/emailactivitysummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_emailactivitysummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.emailActivitySummary not found
Content-type: application/json
Content-length: 206

{
  "@odata.type": "#microsoft.graph.emailActivitySummary",
  "reportRefreshDate": "Date",
  "send": 4,
  "receive": 7,
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
Content-Length: 255

{
  "@odata.type": "#microsoft.graph.emailActivitySummary",
  "id": "f20eee41-ee41-f20e-41ee-0ef241ee0ef2",
  "reportRefreshDate": "Date",
  "send": 4,
  "receive": 7,
  "read": 4,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

