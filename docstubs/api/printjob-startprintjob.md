---
title: "printJob: startPrintJob"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# startPrintJob

Namespace: microsoft.graph



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
POST /print/printers/{printerId}/jobs/{printJobId}/startPrintJob
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "printjob_startprintjob"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}/startPrintJob
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printjobstatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 76

{
  "value": {
    "@odata.type": "microsoft.graph.printJobStatus"
  }
}
```

