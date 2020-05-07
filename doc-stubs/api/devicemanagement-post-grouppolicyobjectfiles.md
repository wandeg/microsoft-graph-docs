---
title: "Create groupPolicyObjectFiles"
description: "Create a new groupPolicyObjectFiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create groupPolicyObjectFiles

Namespace: microsoft.graph

Create a new groupPolicyObjectFiles object.

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
POST /deviceManagement/groupPolicyObjectFiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object.

The following table shows the properties that are required when you create the [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|groupPolicyObjectId|Guid|**TODO: Add Description**|
|ouDistinguishedName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|content|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicyobjectfile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
Content-Type: application/json
Content-length: 157

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "content": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicyobjectfile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "2b581a5a-1a5a-2b58-5a1a-582b5a1a582b",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "content": "String"
}
```

