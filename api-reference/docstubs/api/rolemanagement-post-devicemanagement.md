---
title: "Create deviceManagement"
description: "Create a new deviceManagement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceManagement

Namespace: microsoft.graph

Create a new deviceManagement object.

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
POST /roleManagement/deviceManagement
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.

The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_rbacapplicationmultiple_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-Type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rbacapplicationmultiple"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "f27d6430-6430-f27d-3064-7df230647df2"
}
```

