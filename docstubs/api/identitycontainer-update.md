---
title: "Update identityContainer"
description: "Update the properties of a identityContainer object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update identityContainer

Namespace: microsoft.graph

Update the properties of a [identityContainer](../resources/identitycontainer.md) object.

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
PATCH /identity
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [identityContainer](../resources/identitycontainer.md) object.

The following table shows the properties that are required when you create the [identityContainer](../resources/identitycontainer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [identityContainer](../resources/identitycontainer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_identitycontainer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity
Content-type: application/json
Content-length: 59

{
  "@odata.type": "#microsoft.graph.identityContainer"
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
Content-Length: 108

{
  "@odata.type": "#microsoft.graph.identityContainer",
  "id": "b0b9df22-df22-b0b9-22df-b9b022dfb9b0"
}
```

