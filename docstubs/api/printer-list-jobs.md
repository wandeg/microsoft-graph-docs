---
title: "List jobs"
description: "Get the printJobs from the jobs navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List jobs

Namespace: microsoft.graph

Get the printJobs from the jobs navigation property.

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
GET /print/printers/{printerId}/jobs
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
If successful, this method returns a `200 OK` response code and a collection of [printJob](../resources/printjob.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/jobs
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printjob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printJob",
      "id": "8df51612-1612-8df5-1216-f58d1216f58d",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "status": {
        "@odata.type": "microsoft.graph.printJobStatus",
        "processingState": "String",
        "processingStateDescription": "Processing State Description value",
        "acquiredByPrinter": true
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.userIdentity",
        "id": "Id value",
        "displayName": "Display Name value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      }
    }
  ]
}
```

