---
title: "Create connections"
description: "Create a new connections object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create connections

Namespace: microsoft.graph

Create a new connections object.

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
POST /external/connections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [externalConnection](../resources/externalconnection.md) object.

The following table shows the properties that are required when you create the [externalConnection](../resources/externalconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|configuration|[configuration](../resources/configuration.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [externalConnection](../resources/externalconnection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/beta/external/connections
Content-Type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.externalConnection",
  "name": "Name value",
  "description": "Description value",
  "configuration": {
    "@odata.type": "microsoft.graph.configuration",
    "authorizedApps": [
      "Authorized Apps value"
    ]
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalconnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.externalConnection",
  "id": "dd5ce4d3-e4d3-dd5c-d3e4-5cddd3e45cdd",
  "name": "Name value",
  "description": "Description value",
  "configuration": {
    "@odata.type": "microsoft.graph.configuration",
    "authorizedApps": [
      "Authorized Apps value"
    ]
  }
}
```

