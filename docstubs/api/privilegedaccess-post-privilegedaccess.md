---
title: "Create privilegedAccess"
description: "Create a new privilegedAccess object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedAccess

Namespace: microsoft.graph

Create a new [privilegedAccess](../resources/privilegedaccess.md) object.

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
POST /privilegedAccess
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedAccess](../resources/privilegedaccess.md) object.

The following table shows the properties that are required when you create the [privilegedAccess](../resources/privilegedaccess.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [privilegedAccess](../resources/privilegedaccess.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedaccess_from_privilegedaccess"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedAccess
Content-type: application/json
Content-length: 98

{
  "@odata.type": "#microsoft.graph.privilegedAccess",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedaccess"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 147

{
  "@odata.type": "#microsoft.graph.privilegedAccess",
  "id": "e79a9a98-9a98-e79a-989a-9ae7989a9ae7",
  "displayName": "Display Name value"
}
```

