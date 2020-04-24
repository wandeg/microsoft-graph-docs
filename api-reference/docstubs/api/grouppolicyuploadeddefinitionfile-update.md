---
title: "Update groupPolicyUploadedDefinitionFile"
description: "Update the properties of a groupPolicyUploadedDefinitionFile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupPolicyUploadedDefinitionFile

Namespace: microsoft.graph

Update the properties of a [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.

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
PATCH /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object.

The following table shows the properties that are required when you create the [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The localized friendly name of the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|description|String|The localized description of the policy settings in the ADMX file. The default value is empty. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|languageCodes|String collection|The supported language codes for the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|targetPrefix|String|Specifies the logical name that refers to the namespace within the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|targetNamespace|String|Specifies the URI used to identify the namespace within the ADMX file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|policyType|groupPolicyType|Specifies the type of group policy. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md). Possible values are: `admxBacked`, `admxIngested`.|
|revision|String|The revision version associated with the file. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|
|fileName|String|The file name of the uploaded ADML file.|
|status|groupPolicyUploadedDefinitionFileStatus|The upload status of the uploaded ADMX file. Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|content|Binary|The contents of the uploaded ADMX file.|
|uploadDateTime|DateTimeOffset|The uploaded time of the uploaded ADMX file.|
|defaultLanguageCode|String|The default language of the uploaded ADMX file.|
|groupPolicyUploadedLanguageFiles|[groupPolicyUploadedLanguageFile](../resources/grouppolicyuploadedlanguagefile.md) collection|The list of ADML files associated with the uploaded ADMX file.|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_grouppolicyuploadeddefinitionfile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}
Content-Type: application/json
Content-length: 765

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "String",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "String",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2017-01-01T00:01:55.145768+03:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "languageCode": "Language Code value",
      "id": "Id value"
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
  "id": "0d795e3e-5e3e-0d79-3e5e-790d3e5e790d",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "String",
  "revision": "Revision value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "fileName": "File Name value",
  "status": "String",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2017-01-01T00:01:55.145768+03:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "languageCode": "Language Code value",
      "id": "Id value"
    }
  ]
}
```

