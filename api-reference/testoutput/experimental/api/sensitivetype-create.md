---
title: "Create sensitiveType"
description: "Create a new sensitiveType object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sensitiveType

Namespace: microsoft.graph

Create a new [sensitiveType](../resources/sensitivetype.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /dataClassification/sensitiveTypes
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [sensitiveType](../resources/sensitivetype.md) object.

The following table shows the properties that are required when you create the [sensitiveType](../resources/sensitivetype.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|description|String||
|rulePackageId|String||
|rulePackageType|String||
|publisherName|String||
|state|String||
|scope|Enumeration|. Possible values are: `fullDocument`, `partialDocument`.|



## Response
If successful, this method returns a `201 Created` response code and a [sensitiveType](../resources/sensitivetype.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sensitivetype_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/dataClassification/sensitiveTypes
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.sensitiveType",
  "name": "Name value",
  "description": "Description value",
  "rulePackageId": "Rule Package Id value",
  "rulePackageType": "Rule Package Type value",
  "publisherName": "Publisher Name value",
  "state": "State value",
  "scope": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivetype"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.sensitiveType",
  "id": "c2d268be-68be-c2d2-be68-d2c2be68d2c2",
  "name": "Name value",
  "description": "Description value",
  "rulePackageId": "Rule Package Id value",
  "rulePackageType": "Rule Package Type value",
  "publisherName": "Publisher Name value",
  "state": "State value",
  "scope": "String"
}
```

