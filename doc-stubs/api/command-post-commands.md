---
title: "Create command"
description: "Create a new command object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create command

Namespace: microsoft.graph

Create a new [command](../resources/command.md) object.

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
POST /commands
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [command](../resources/command.md) object.

The following table shows the properties that are required when you create the [command](../resources/command.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|Status|String|**TODO: Add Description**|
|Type|String|**TODO: Add Description**|
|AppServiceName|String|**TODO: Add Description**|
|PackageFamilyName|String|**TODO: Add Description**|
|Error|String|**TODO: Add Description**|
|Payload|[PayloadRequest](../resources/payloadrequest.md)|**TODO: Add Description**|
|PermissionTicket|String|**TODO: Add Description**|
|PostBackUri|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [command](../resources/command.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_command_from_commands"
}
-->
``` http
POST https://graph.microsoft.com/beta/commands
Content-Type: application/json
Content-length: 316

{
  "@odata.type": "#microsoft.graph.command",
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
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

