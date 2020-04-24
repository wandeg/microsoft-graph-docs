---
title: "Create managementConditionStatements"
description: "Create a new managementConditionStatements object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managementConditionStatements

Namespace: microsoft.graph

Create a new managementConditionStatements object.

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
POST /deviceManagement/managementConditionStatements
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [managementConditionStatement](../resources/managementconditionstatement.md) object.

The following table shows the properties that are required when you create the [managementConditionStatement](../resources/managementconditionstatement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The admin defined name of the management condition statement.|
|description|String|The admin defined description of the management condition statement.|
|createdDateTime|DateTimeOffset|The time the management condition statement was created. Generated service side.|
|modifiedDateTime|DateTimeOffset|The time the management condition statement was last modified. Updated service side.|
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)|The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.|
|eTag|String|ETag of the management condition statement. Updated service side.|
|applicablePlatforms|devicePlatformType collection|The applicable platforms for this management condition statement.
This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|



## Response
If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/managementconditionstatement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managementconditionstatement_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-Type: application/json
Content-length: 315

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managementconditionstatement"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "d1704d60-4d60-d170-604d-70d1604d70d1",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

