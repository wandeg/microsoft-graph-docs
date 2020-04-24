---
title: "List groupPolicyUploadedDefinitionFiles"
description: "Get the groupPolicyUploadedDefinitionFiles from the groupPolicyUploadedDefinitionFiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List groupPolicyUploadedDefinitionFiles

Namespace: microsoft.graph

Get the groupPolicyUploadedDefinitionFiles from the groupPolicyUploadedDefinitionFiles navigation property.

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
GET /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinitionFile](../resources/grouppolicyuploadeddefinitionfile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_grouppolicyuploadeddefinitionfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicyuploadeddefinitionfile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

