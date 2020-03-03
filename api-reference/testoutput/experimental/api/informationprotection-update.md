---
title: "Update informationProtection"
description: "Update the properties of a informationProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update informationProtection

Namespace: microsoft.graph

Update the properties of a [informationProtection](../resources/informationprotection.md) object.

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
PATCH /informationProtection
PATCH /me/informationProtection
PATCH /users/{usersId}/informationProtection
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [informationProtection](../resources/informationprotection.md) object.

The following table shows the properties that are required when you create the [informationProtection](../resources/informationprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [informationProtection](../resources/informationprotection.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_informationprotection"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/informationProtection
Content-type: application/json
Content-length: 63

{
  "@odata.type": "#microsoft.graph.informationProtection"
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
Content-Length: 112

{
  "@odata.type": "#microsoft.graph.informationProtection",
  "id": "1f44737b-737b-1f44-7b73-441f7b73441f"
}
```

