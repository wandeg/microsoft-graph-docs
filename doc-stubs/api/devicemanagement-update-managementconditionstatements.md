---
title: "Update managementConditionStatements"
description: "Update the properties of a managementConditionStatements object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managementConditionStatements

Namespace: microsoft.graph

Update the properties of a managementConditionStatements object.

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
PATCH /deviceManagement/managementConditionStatements
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managementConditionStatement](../resources/managementconditionstatement.md) object.

The following table shows the properties that are required when you create the [managementConditionStatement](../resources/managementconditionstatement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)|**TODO: Add Description**|
|eTag|String|**TODO: Add Description**|
|applicablePlatforms|devicePlatformType collection|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/managementconditionstatement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managementconditionstatements"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-Type: application/json
Content-length: 288

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "String",
  "description": "String",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
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
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "6c6ef364-f364-6c6e-64f3-6e6c64f36e6c",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```

