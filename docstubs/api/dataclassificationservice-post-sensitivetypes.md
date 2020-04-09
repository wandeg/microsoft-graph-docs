---
title: "Add sensitiveTypes"
description: "Add sensitiveTypes by posting to the sensitiveTypes collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add sensitiveTypes

Namespace: microsoft.graph

Add sensitiveTypes by posting to the sensitiveTypes collection.

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
POST /dataClassification/sensitiveTypes/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
|scope|Enumeration| Possible values are: `fullDocument`, `partialDocument`.|



## Response
If successful, this method returns a `201 Created` response code and a [sensitiveType](../resources/sensitivetype.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sensitivetype_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/sensitiveTypes
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
  "id": "bd9ba954-a954-bd9b-54a9-9bbd54a99bbd",
  "name": "Name value",
  "description": "Description value",
  "rulePackageId": "Rule Package Id value",
  "rulePackageType": "Rule Package Type value",
  "publisherName": "Publisher Name value",
  "state": "State value",
  "scope": "String"
}
```

