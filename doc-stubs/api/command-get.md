---
title: "Get command"
description: "Read the properties and relationships of a command object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get command

Namespace: microsoft.graph

Read the properties and relationships of a [command](../resources/command.md) object.

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
GET /commands/{commandsId}
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

If successful, this method returns a `200 OK` response code and a [command](../resources/command.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_command"
}
-->
``` http
GET https://graph.microsoft.com/beta/commands/{commandsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.command"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.command",
    "id": "6ac9ad66-ad66-6ac9-66ad-c96a66adc96a",
    "Status": "String",
    "Type": "String",
    "AppServiceName": "String",
    "PackageFamilyName": "String",
    "Error": "String",
    "Payload": {
      "@odata.type": "microsoft.graph.PayloadRequest"
    },
    "PermissionTicket": "String",
    "PostBackUri": "String"
  }
}
```

