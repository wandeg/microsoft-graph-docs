---
title: "Create conditionalAccess"
description: "Create a new conditionalAccess object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create conditionalAccess

Namespace: microsoft.graph

Create a new conditionalAccess object.

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
POST /identity/conditionalAccess
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.

The following table shows the properties that are required when you create the [conditionalAccessRoot](../resources/conditionalaccessroot.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccessroot_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identity/conditionalAccess
Content-Type: application/json
Content-length: 63

{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalaccessroot"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot",
  "id": "0776bc6c-bc6c-0776-6cbc-76076cbc7607"
}
```

