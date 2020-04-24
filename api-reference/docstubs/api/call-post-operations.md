---
title: "Create operations"
description: "Create a new operations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create operations

Namespace: microsoft.graph

Create a new operations object.

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
POST /communications/calls/{callId}/operations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [commsOperation](../resources/commsoperation.md) object.

The following table shows the properties that are required when you create the [commsOperation](../resources/commsoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|operationStatus|**TODO: Add Description**. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|clientContext|String|**TODO: Add Description**|
|resultInfo|[ResultInfo](../resources/resultinfo.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_commsoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/calls/{callId}/operations
Content-Type: application/json
Content-length: 265

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.commsOperation",
  "id": "b571cdaa-cdaa-b571-aacd-71b5aacd71b5",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  }
}
```

