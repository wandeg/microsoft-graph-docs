---
title: "Update jobs"
description: "Update the properties of a jobs object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update jobs

Namespace: microsoft.graph

Update the properties of a jobs object.

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
PATCH /print/printers/{printerId}/jobs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [printJob](../resources/printjob.md) object.

The following table shows the properties that are required when you create the [printJob](../resources/printjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|status|[printJobStatus](../resources/printjobstatus.md)|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [printJob](../resources/printjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_jobs"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printers/{printerId}/jobs
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

