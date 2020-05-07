---
title: "Create deviceEnrollmentConfigurations"
description: "Create a new deviceEnrollmentConfigurations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceEnrollmentConfigurations

Namespace: microsoft.graph

Create a new deviceEnrollmentConfigurations object.

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
POST /me/deviceEnrollmentConfigurations
POST /users/{usersId}/deviceEnrollmentConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deviceenrollmentconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/deviceEnrollmentConfigurations
Content-Type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "version": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceenrollmentconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "e5a7836b-836b-e5a7-6b83-a7e56b83a7e5",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer"
}
```

