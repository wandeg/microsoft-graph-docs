---
title: "List regionalAndLanguageSettings"
description: "Get a list of the regionalAndLanguageSettings objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List regionalAndLanguageSettings

Namespace: microsoft.graph

Get a list of the [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.regionalAndLanguageSettings not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_regionalandlanguagesettings"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.regionalAndLanguageSettings not found
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.regionalandlanguagesettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.regionalAndLanguageSettings",
      "id": "a8e68d5b-8d5b-a8e6-5b8d-e6a85b8de6a8",
      "defaultDisplayLanguage": {
        "@odata.type": "microsoft.graph.localeInfo"
      },
      "authoringLanguages": [
        {
          "@odata.type": "microsoft.graph.localeInfo"
        }
      ],
      "defaultTranslationLanguage": {
        "@odata.type": "microsoft.graph.localeInfo"
      },
      "defaultSpeechInputLanguage": {
        "@odata.type": "microsoft.graph.localeInfo"
      },
      "defaultRegionalFormat": {
        "@odata.type": "microsoft.graph.localeInfo"
      },
      "regionalFormatOverrides": {
        "@odata.type": "microsoft.graph.regionalFormatOverrides"
      }
    }
  ]
}
```

