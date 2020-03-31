---
title: "Create externalConnection"
description: "Create a new externalConnection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create externalConnection

Namespace: microsoft.graph

Create a new [externalConnection](../resources/externalconnection.md) object.

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
POST /connections
POST /external/connections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [externalConnection](../resources/externalconnection.md) object.

The following table shows the properties that are required when you create the [externalConnection](../resources/externalconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|description|String||
|configuration|[configuration](../resources/configuration.md)||



## Response
If successful, this method returns a `201 Created` response code and a [externalConnection](../resources/externalconnection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/beta/connections
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalconnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.externalConnection",
  "id": "3cee3cc1-3cc1-3cee-c13c-ee3cc13cee3c",
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

