---
title: "Update groupPolicyUploadedDefinitionFiles"
description: "Update the properties of a groupPolicyUploadedDefinitionFiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupPolicyUploadedDefinitionFiles

Namespace: microsoft.graph

Update the properties of a groupPolicyUploadedDefinitionFiles object.

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
PATCH /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.

The following table shows the properties that are required when you create the [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|description|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|languageCodes|String collection|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|targetPrefix|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|targetNamespace|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|policyType|groupPolicyType|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md). Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|fileName|String|**TODO: Add Description**|
|status|groupPolicyUploadedDefinitionFileStatus|**TODO: Add Description**. Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|content|Binary|**TODO: Add Description**|
|uploadDateTime|DateTimeOffset|**TODO: Add Description**|
|defaultLanguageCode|String|**TODO: Add Description**|
|groupPolicyUploadedLanguageFiles|[groupPolicyUploadedLanguageFile](../resources/grouppolicyuploadedlanguagefile.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_grouppolicyuploadeddefinitionfiles"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
Content-Type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "fileName": "String",
  "status": "String",
  "content": "Binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
    }
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
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "id": "0d057839-7839-0d05-3978-050d3978050d",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "status": "String",
  "content": "Binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
    }
  ]
}
```

