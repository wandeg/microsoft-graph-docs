---
title: "Add embeddedSIMActivationCodePools"
description: "Add embeddedSIMActivationCodePools by posting to the embeddedSIMActivationCodePools collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add embeddedSIMActivationCodePools

Namespace: microsoft.graph

Add embeddedSIMActivationCodePools by posting to the embeddedSIMActivationCodePools collection.

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
POST /deviceManagement/embeddedSIMActivationCodePools/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.

The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|activationCodes|[embeddedSIMActivationCode](../resources/embeddedsimactivationcode.md) collection||
|activationCodeCount|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_embeddedsimactivationcodepool_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.embeddedsimactivationcodepool"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "8fd4da0c-da0c-8fd4-0cda-d48f0cdad48f",
  "displayName": "Display Name value",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "modifiedDateTime": "2016-12-31T23:57:56.5934914+03:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

