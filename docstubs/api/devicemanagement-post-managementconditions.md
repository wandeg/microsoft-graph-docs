---
title: "Add managementConditions"
description: "Add managementConditions by posting to the managementConditions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add managementConditions

Namespace: microsoft.graph

Add managementConditions by posting to the managementConditions collection.

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
POST /deviceManagement/managementConditions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managementCondition](../resources/managementcondition.md) object.

The following table shows the properties that are required when you create the [managementCondition](../resources/managementcondition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|uniqueName|String||
|displayName|String||
|description|String||
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|eTag|String||
|applicablePlatforms|Enumeration collection| Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|



## Response
If successful, this method returns a `201 Created` response code and a [managementCondition](../resources/managementcondition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managementcondition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.managementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managementcondition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "ae6da4be-a4be-ae6d-bea4-6daebea46dae",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "modifiedDateTime": "2017-01-01T00:01:10.7827862+00:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

