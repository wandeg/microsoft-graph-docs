---
title: "Create informationProtectionPolicy"
description: "Create a new informationProtectionPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create informationProtectionPolicy

Namespace: microsoft.graph

Create a new [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.

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
POST ** Collection URI for microsoft.graph.informationProtectionPolicy not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.

The following table shows the properties that are required when you create the [informationProtectionPolicy](../resources/informationprotectionpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_informationprotectionpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.informationProtectionPolicy not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.informationprotectionpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 118

{
  "@odata.type": "#microsoft.graph.informationProtectionPolicy",
  "id": "738d216e-216e-738d-6e21-8d736e218d73"
}
```

