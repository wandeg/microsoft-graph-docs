---
title: "Create roleDefinitions"
description: "Create a new roleDefinitions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create roleDefinitions

Namespace: microsoft.graph

Create a new roleDefinitions object.

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
POST ** Collection URI for microsoft.graph.governanceRoleDefinition not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.

The following table shows the properties that are required when you create the [governanceRoleDefinition](../resources/governanceroledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceId|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governanceroledefinition_from_governanceroledefinitions"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.governanceRoleDefinition not found
Content-Type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "resourceId": "String",
  "externalId": "String",
  "templateId": "String",
  "displayName": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceroledefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "id": "0bac15b1-15b1-0bac-b115-ac0bb115ac0b",
  "resourceId": "String",
  "externalId": "String",
  "templateId": "String",
  "displayName": "String"
}
```

