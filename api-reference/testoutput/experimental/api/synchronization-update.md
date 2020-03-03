---
title: "Update synchronization"
description: "Update the properties of a synchronization object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update synchronization

Update the properties of a [synchronization](../resources/synchronization.md) object.

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
PATCH /applications/{applicationsId}/synchronization
PATCH /servicePrincipals/{servicePrincipalsId}/synchronization
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [synchronization](../resources/synchronization.md) object.

The following table shows the properties that are required when you create the [synchronization](../resources/synchronization.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|secrets|[synchronizationSecretKeyStringValuePair](../resources/synchronizationSecretKeyStringValuePair.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [synchronization](../resources/synchronization.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_synchronization"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/applications/{applicationsId}/synchronization
Content-type: application/json
Content-length: 228

{
  "@odata.type": "#microsoft.graph.synchronization",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair",
      "key": "String",
      "value": "Value value"
    }
  ]
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
Content-Length: 277

{
  "@odata.type": "#microsoft.graph.synchronization",
  "id": "a7731f6c-1f6c-a773-6c1f-73a76c1f73a7",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair",
      "key": "String",
      "value": "Value value"
    }
  ]
}
```

