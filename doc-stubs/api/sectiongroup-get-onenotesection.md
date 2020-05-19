---
title: "Get sections"
description: "Read the properties and relationships of an onenoteSection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get sections

Namespace: microsoft.graph

Read the properties and relationships of an [onenoteSection](../resources/onenotesection.md) object.

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
GET /users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections
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

If successful, this method returns a `200 OK` response code and an [onenoteSection](../resources/onenotesection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onenotesection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteSection",
    "id": "b5bb53da-53da-b5bb-da53-bbb5da53bbb5",
    "self": "String",
    "createdDateTime": "String (timestamp)",
    "displayName": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "isDefault": "Boolean",
    "links": {
      "@odata.type": "microsoft.graph.sectionLinks"
    },
    "pagesUrl": "String"
  }
}
```

