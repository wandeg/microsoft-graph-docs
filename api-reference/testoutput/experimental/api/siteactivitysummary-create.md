---
title: "Create siteActivitySummary"
description: "Create a new siteActivitySummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create siteActivitySummary

Namespace: microsoft.graph

Create a new [siteActivitySummary](../resources/siteactivitysummary.md) object.

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
POST ** Collection URI for microsoft.graph.siteActivitySummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [siteActivitySummary](../resources/siteactivitysummary.md) object.

The following table shows the properties that are required when you create the [siteActivitySummary](../resources/siteactivitysummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|viewedOrEdited|Int64||
|synced|Int64||
|sharedInternally|Int64||
|sharedExternally|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [siteActivitySummary](../resources/siteactivitysummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_siteactivitysummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.siteActivitySummary not found
Content-type: application/json
Content-length: 253

{
  "@odata.type": "#microsoft.graph.siteActivitySummary",
  "reportRefreshDate": "Date",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.siteactivitysummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 302

{
  "@odata.type": "#microsoft.graph.siteActivitySummary",
  "id": "1795a129-a129-1795-29a1-951729a19517",
  "reportRefreshDate": "Date",
  "viewedOrEdited": 14,
  "synced": 6,
  "sharedInternally": 0,
  "sharedExternally": 0,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

