---
title: "List siteActivitySummaries"
description: "List properties and relationships of the siteActivitySummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List siteActivitySummaries

Namespace: microsoft.graph

List properties and relationships of the [siteActivitySummary](../resources/siteactivitysummary.md) objects.

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
GET ** Collection URI for microsoft.graph.siteActivitySummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [siteActivitySummary](../resources/siteactivitysummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_siteactivitysummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.siteActivitySummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.siteactivitysummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "value": [
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
  ]
}
```

