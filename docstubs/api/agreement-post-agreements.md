---
title: "Create agreement"
description: "Create a new agreement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create agreement

Namespace: microsoft.graph

Create a new [agreement](../resources/agreement.md) object.

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
POST /agreements
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [agreement](../resources/agreement.md) object.

The following table shows the properties that are required when you create the [agreement](../resources/agreement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|isViewingBeforeAcceptanceRequired|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [agreement](../resources/agreement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}
-->
``` http
POST https://graph.microsoft.com/beta/agreements
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.agreement",
  "displayName": "Display Name value",
  "isViewingBeforeAcceptanceRequired": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "e873a2c3-a2c3-e873-c3a2-73e8c3a273e8",
  "displayName": "Display Name value",
  "isViewingBeforeAcceptanceRequired": true
}
```

