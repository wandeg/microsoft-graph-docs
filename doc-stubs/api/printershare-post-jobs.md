---
title: "Create jobs"
description: "Create a new jobs object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create jobs

Namespace: microsoft.graph

Create a new jobs object.

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
POST /print/printers/{printerId}/share/jobs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/share/jobs
Content-Type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.printJob",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printjob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

