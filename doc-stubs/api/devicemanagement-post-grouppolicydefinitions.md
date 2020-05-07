---
title: "Create groupPolicyDefinitions"
description: "Create a new groupPolicyDefinitions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create groupPolicyDefinitions

Namespace: microsoft.graph

Create a new groupPolicyDefinitions object.

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
POST /deviceManagement/groupPolicyDefinitions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.

The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/grouppolicydefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|classType|groupPolicyDefinitionClassType|**TODO: Add Description**. Possible values are: `user`, `machine`.|
|displayName|String|**TODO: Add Description**|
|explainText|String|**TODO: Add Description**|
|categoryPath|String|**TODO: Add Description**|
|supportedOn|String|**TODO: Add Description**|
|policyType|groupPolicyType|**TODO: Add Description**. Possible values are: `admxBacked`, `admxIngested`.|
|groupPolicyCategoryId|Guid|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
Content-Type: application/json
Content-length: 265

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicydefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "id": "3ff9d3d5-d3d5-3ff9-d5d3-f93fd5d3f93f",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid",
  "lastModifiedDateTime": "String (timestamp)"
}
```

