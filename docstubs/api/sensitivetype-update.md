---
title: "Update sensitiveType"
description: "Update the properties of a sensitiveType object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sensitiveType

Namespace: microsoft.graph

Update the properties of a [sensitiveType](../resources/sensitivetype.md) object.

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
PATCH /dataClassification/sensitiveTypes/{sensitiveTypeId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [sensitiveType](../resources/sensitivetype.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sensitivetype"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/sensitiveTypes/{sensitiveTypeId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.sensitiveType",
  "id": "a1f50f99-0f99-a1f5-990f-f5a1990ff5a1",
  "name": "Name value",
  "description": "Description value",
  "rulePackageId": "Rule Package Id value",
  "rulePackageType": "Rule Package Type value",
  "publisherName": "Publisher Name value",
  "state": "State value",
  "scope": "String"
}
```

