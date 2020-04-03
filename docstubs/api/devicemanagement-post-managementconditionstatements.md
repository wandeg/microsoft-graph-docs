---
title: "Add managementConditionStatements"
description: "Add managementConditionStatements by posting to the managementConditionStatements collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add managementConditionStatements

Namespace: microsoft.graph

Add managementConditionStatements by posting to the managementConditionStatements collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managementConditionStatement](../resources/managementconditionstatement.md) object.

The following table shows the properties that are required when you create the [managementConditionStatement](../resources/managementconditionstatement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)||
|eTag|String||
|applicablePlatforms|Enumeration collection| Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|



## Response
If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/managementconditionstatement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managementconditionstatement_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managementconditionstatement"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "ba90a02b-a02b-ba90-2ba0-90ba2ba090ba",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "modifiedDateTime": "2016-12-31T23:58:55.6791311+00:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

