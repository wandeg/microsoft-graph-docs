---
title: "Create ndesConnectors"
description: "Create a new ndesConnectors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create ndesConnectors

Namespace: microsoft.graph

Create a new ndesConnectors object.

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
POST /deviceManagement/ndesConnectors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [ndesConnector](../resources/ndesconnector.md) object.

The following table shows the properties that are required when you create the [ndesConnector](../resources/ndesconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Last connection time for the Ndes Connector|
|state|ndesConnectorState|Ndes Connector Status. Possible values are: `none`, `active`, `inactive`.|
|displayName|String|The friendly name of the Ndes Connector.|



## Response
If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/ndesconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_ndesconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-Type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:57:28.9541214+03:00",
  "state": "String",
  "displayName": "Display Name value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ndesconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "11ecbb9e-bb9e-11ec-9ebb-ec119ebbec11",
  "lastConnectionDateTime": "2016-12-31T23:57:28.9541214+03:00",
  "state": "String",
  "displayName": "Display Name value"
}
```

