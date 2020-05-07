---
title: "Get printJob"
description: "Read the properties and relationships of a printJob object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get printJob

Namespace: microsoft.graph

Read the properties and relationships of a [printJob](../resources/printjob.md) object.

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
GET /print/printers/{printerId}/jobs/{printJobId}
GET /print/printers/{printerId}/share/jobs/{printJobId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.printJob",
    "id": "6640a0cc-a0cc-6640-cca0-4066cca04066",
    "createdDateTime": "String (timestamp)",
    "status": {
      "@odata.type": "microsoft.graph.printJobStatus"
    },
    "createdBy": {
      "@odata.type": "microsoft.graph.userIdentity"
    }
  }
}
```

