---
title: "List parentSectionGroup"
description: "Get the sectionGroups from the parentSectionGroup navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List parentSectionGroup

Namespace: microsoft.graph

Get the sectionGroups from the parentSectionGroup navigation property.

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
GET /users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/parentSectionGroup
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

If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/parentSectionGroup
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sectiongroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sectionGroup",
      "id": "f6e215d7-15d7-f6e2-d715-e2f6d715e2f6",
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
      "sectionsUrl": "String",
      "sectionGroupsUrl": "String"
    }
  ]
}
```

