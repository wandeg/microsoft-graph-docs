---
title: "Update printJob"
description: "Update the properties of a printJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update printJob

Namespace: microsoft.graph

Update the properties of a [printJob](../resources/printjob.md) object.

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
PATCH /print/printers/{printerId}/jobs/{printJobId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [printJob](../resources/printjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_printjob"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 604

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
```

