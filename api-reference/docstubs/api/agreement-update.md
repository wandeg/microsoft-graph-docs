---
title: "Update agreement"
description: "Update the properties of an agreement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update agreement

Namespace: microsoft.graph

Update the properties of an [agreement](../resources/agreement.md) object.

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
PATCH /agreements/{agreementsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.

The following table shows the properties that are required when you create the [agreement](../resources/agreement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|isViewingBeforeAcceptanceRequired|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/agreements/{agreementsId}
Content-Type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.agreement",
  "displayName": "Display Name value",
  "isViewingBeforeAcceptanceRequired": true
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
  "@odata.type": "#microsoft.graph.agreement",
  "id": "4cb72093-2093-4cb7-9320-b74c9320b74c",
  "displayName": "Display Name value",
  "isViewingBeforeAcceptanceRequired": true
}
```

