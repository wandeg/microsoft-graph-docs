---
title: "Update informationProtectionPolicy"
description: "Update the properties of a informationProtectionPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update informationProtectionPolicy

Namespace: microsoft.graph

Update the properties of a [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.

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
PATCH /informationProtection/policy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.

The following table shows the properties that are required when you create the [informationProtectionPolicy](../resources/informationprotectionpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_informationprotectionpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/informationProtection/policy
Content-type: application/json
Content-length: 69

{
  "@odata.type": "#microsoft.graph.informationProtectionPolicy"
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
Content-Length: 118

{
  "@odata.type": "#microsoft.graph.informationProtectionPolicy",
  "id": "b773f83f-f83f-b773-3ff8-73b73ff873b7"
}
```

