---
title: "Create ndesConnector"
description: "Create a new ndesConnector object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create ndesConnector

Namespace: microsoft.graph

Create a new [ndesConnector](../resources/ndesconnector.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [ndesConnector](../resources/ndesconnector.md) object.

The following table shows the properties that are required when you create the [ndesConnector](../resources/ndesconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Last connection time for the Ndes Connector|
|state|Enumeration|Ndes Connector Status. Possible values are: `none`, `active`, `inactive`.|
|displayName|String|The friendly name of the Ndes Connector.|



## Response
If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/ndesconnector.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_ndesconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:56:25.4273633+03:00",
  "state": "String",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ndesconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "963deb66-eb66-963d-66eb-3d9666eb3d96",
  "lastConnectionDateTime": "2016-12-31T23:56:25.4273633+03:00",
  "state": "String",
  "displayName": "Display Name value"
}
```

