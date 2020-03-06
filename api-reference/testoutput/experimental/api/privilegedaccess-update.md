---
title: "Update privilegedAccess"
description: "Update the properties of a privilegedAccess object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedAccess

Namespace: microsoft.graph

Update the properties of a [privilegedAccess](../resources/privilegedaccess.md) object.

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
PATCH /privilegedAccess/{privilegedAccessId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedAccess](../resources/privilegedaccess.md) object.

The following table shows the properties that are required when you create the [privilegedAccess](../resources/privilegedaccess.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedAccess](../resources/privilegedaccess.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedaccess"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/privilegedAccess/{privilegedAccessId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 147

{
  "@odata.type": "#microsoft.graph.privilegedAccess",
  "id": "3aaaf363-f363-3aaa-63f3-aa3a63f3aa3a",
  "displayName": "Display Name value"
}
```

