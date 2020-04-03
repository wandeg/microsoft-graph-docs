---
title: "Update embeddedSIMActivationCodePool"
description: "Update the properties of a embeddedSIMActivationCodePool object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update embeddedSIMActivationCodePool

Namespace: microsoft.graph

Update the properties of a [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.

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
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_embeddedsimactivationcodepool"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "b4929d3a-9d3a-b492-3a9d-92b43a9d92b4",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "modifiedDateTime": "2016-12-31T23:58:55.6791311+00:00",
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

