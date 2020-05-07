---
title: "Update groupPolicyConfigurations"
description: "Update the properties of a groupPolicyConfigurations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupPolicyConfigurations

Namespace: microsoft.graph

Update the properties of a groupPolicyConfigurations object.

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
PATCH /deviceManagement/groupPolicyConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.

The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_grouppolicyconfigurations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
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
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "id": "e57be9de-e9de-e57b-dee9-7be5dee97be5",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "lastModifiedDateTime": "String (timestamp)"
}
```

