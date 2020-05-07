---
title: "Update definitionValues"
description: "Update the properties of a definitionValues object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update definitionValues

Namespace: microsoft.graph

Update the properties of a definitionValues object.

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
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.

The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|configurationType|groupPolicyConfigurationType|**TODO: Add Description**. Possible values are: `policy`, `preference`.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_definitionvalues"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-Type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": "Boolean",
  "configurationType": "String"
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
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "id": "5d9f8c5b-8c5b-5d9f-5b8c-9f5d5b8c9f5d",
  "createdDateTime": "String (timestamp)",
  "enabled": "Boolean",
  "configurationType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

