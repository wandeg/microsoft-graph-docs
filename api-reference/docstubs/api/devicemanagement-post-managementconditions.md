---
title: "Create managementConditions"
description: "Create a new managementConditions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managementConditions

Namespace: microsoft.graph

Create a new managementConditions object.

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
POST /deviceManagement/managementConditions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [managementCondition](../resources/managementcondition.md) object.

The following table shows the properties that are required when you create the [managementCondition](../resources/managementcondition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions.|
|displayName|String|The admin defined name of the management condition.|
|description|String|The admin defined description of the management condition.|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side.|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side.|
|eTag|String|ETag of the management condition. Updated service side.|
|applicablePlatforms|devicePlatformType collection|The applicable platforms for this management condition. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|



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
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managementcondition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "2b26131e-131e-2b26-1e13-262b1e13262b",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ]
}
```

