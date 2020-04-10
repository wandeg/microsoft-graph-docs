---
title: "Add jobs"
description: "Add jobs by posting to the jobs collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add jobs

Namespace: microsoft.graph

Add jobs by posting to the jobs collection.

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
POST /print/printers/{printerId}/jobs/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [printJob](../resources/printjob.md) object.

The following table shows the properties that are required when you create the [printJob](../resources/printjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|status|[printJobStatus](../resources/printjobstatus.md)||
|createdBy|[userIdentity](../resources/useridentity.md)||



## Response
If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/jobs
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.printJob",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printjob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "6ae0ff67-ff67-6ae0-67ff-e06a67ffe06a",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
```

