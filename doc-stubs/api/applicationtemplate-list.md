---
title: "List applicationTemplates"
description: "Get a list of the applicationTemplate objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List applicationTemplates

Namespace: microsoft.graph

Get a list of the [applicationTemplate](../resources/applicationtemplate.md) objects and their properties.

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
GET /applicationTemplates
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

If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/applicationTemplates
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.applicationtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applicationTemplate",
      "id": "73303daa-3daa-7330-aa3d-3073aa3d3073",
      "displayName": "String",
      "homePageUrl": "String",
      "supportedSingleSignOnModes": [
        "String"
      ],
      "supportedProvisioningTypes": [
        "String"
      ],
      "logoUrl": "String",
      "categories": [
        "String"
      ],
      "publisher": "String",
      "description": "String"
    }
  ]
}
```

