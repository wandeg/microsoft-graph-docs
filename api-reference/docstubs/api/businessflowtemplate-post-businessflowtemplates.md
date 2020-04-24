---
title: "Create businessFlowTemplate"
description: "Create a new businessFlowTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create businessFlowTemplate

Namespace: microsoft.graph

Create a new [businessFlowTemplate](../resources/businessflowtemplate.md) object.

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
POST /businessFlowTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [businessFlowTemplate](../resources/businessflowtemplate.md) object.

The following table shows the properties that are required when you create the [businessFlowTemplate](../resources/businessflowtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [businessFlowTemplate](../resources/businessflowtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_businessflowtemplate_from_businessflowtemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/businessFlowTemplates
Content-Type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.businessFlowTemplate",
  "displayName": "Display Name value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessflowtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.businessFlowTemplate",
  "id": "5b953b83-3b83-5b95-833b-955b833b955b",
  "displayName": "Display Name value"
}
```

