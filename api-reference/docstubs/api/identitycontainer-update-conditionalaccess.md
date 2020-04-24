---
title: "Update conditionalAccess"
description: "Update the properties of a conditionalAccess object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update conditionalAccess

Namespace: microsoft.graph

Update the properties of a conditionalAccess object.

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
PATCH /identity/conditionalAccess
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
If successful, this method returns a `200 OK` response code and an updated [conditionalAccessRoot](../resources/conditionalaccessroot.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccess"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot",
  "id": "0776bc6c-bc6c-0776-6cbc-76076cbc7607"
}
```

