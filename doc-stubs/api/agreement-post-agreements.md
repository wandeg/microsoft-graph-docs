---
title: "Create agreement"
description: "Create a new agreement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create agreement

Namespace: microsoft.graph

Create a new [agreement](../resources/agreement.md) object.

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
POST /agreements
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.

The following table shows the properties that are required when you create the [agreement](../resources/agreement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|isViewingBeforeAcceptanceRequired|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [agreement](../resources/agreement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}
-->
``` http
POST https://graph.microsoft.com/beta/agreements
Content-Type: application/json
Content-length: 130

{
  "@odata.type": "#microsoft.graph.agreement",
  "displayName": "String",
  "isViewingBeforeAcceptanceRequired": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "b4e37c8e-7c8e-b4e3-8e7c-e3b48e7ce3b4",
  "displayName": "String",
  "isViewingBeforeAcceptanceRequired": "Boolean"
}
```

