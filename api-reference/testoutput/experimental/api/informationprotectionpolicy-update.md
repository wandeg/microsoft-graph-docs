---
title: "Update informationProtectionPolicy"
description: "Update the properties of a informationProtectionPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update informationProtectionPolicy

Update the properties of a [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.

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
PATCH /informationProtection/policy
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [informationProtectionPolicy](../resources/informationProtectionPolicy.md) object.

The following table shows the properties that are required when you create the [informationProtectionPolicy](../resources/informationprotectionpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_informationprotectionpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/informationProtection/policy
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
  "id": "88172d2c-2d2c-8817-2c2d-17882c2d1788"
}
```

