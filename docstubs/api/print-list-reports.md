---
title: "List reports"
description: "Get the reportRoots from the reports navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List reports

Namespace: microsoft.graph

Get the reportRoots from the reports navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/reports
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [reportRoot](../resources/reportroot.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_reportroot"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/reports
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.reportroot)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 142

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.reportRoot",
      "id": "edb040d0-40d0-edb0-d040-b0edd040b0ed"
    }
  ]
}
```

