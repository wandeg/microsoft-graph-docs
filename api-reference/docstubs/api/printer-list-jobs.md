---
title: "List jobs"
description: "Get the printJobs from the jobs navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List jobs

Namespace: microsoft.graph

Get the printJobs from the jobs navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [printJob](../resources/printjob.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/jobs
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printjob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printJob",
      "id": "9d2d110d-110d-9d2d-0d11-2d9d0d112d9d",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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

