---
title: "Update embeddedSIMActivationCodePools"
description: "Update the properties of an embeddedSIMActivationCodePools object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update embeddedSIMActivationCodePools

Namespace: microsoft.graph

Update the properties of an embeddedSIMActivationCodePools object.

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
PATCH /deviceManagement/embeddedSIMActivationCodePools
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.

The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|activationCodes|[embeddedSIMActivationCode](../resources/embeddedsimactivationcode.md) collection|**TODO: Add Description**|
|activationCodeCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_embeddedsimactivationcodepools"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
Content-Type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "String",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
    }
  ],
  "activationCodeCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "9e9ed176-d176-9e9e-76d1-9e9e76d19e9e",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
    }
  ],
  "activationCodeCount": "Integer"
}
```

