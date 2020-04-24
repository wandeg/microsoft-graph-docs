---
title: "List parentNotebook"
description: "Get the notebooks from the parentNotebook navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List parentNotebook

Namespace: microsoft.graph

Get the notebooks from the parentNotebook navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentNotebook
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
If successful, this method returns a `200 OK` response code and a collection of [notebook](../resources/notebook.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentNotebook
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.notebook)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notebook",
      "id": "23f6b32c-b32c-23f6-2cb3-f6232cb3f623",
      "self": "Self value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "displayName": "Display Name value",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
      "isDefault": true,
      "userRole": "String",
      "isShared": true,
      "sectionsUrl": "https://example.com/sectionsUrl/",
      "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/",
      "links": {
        "@odata.type": "microsoft.graph.notebookLinks",
        "oneNoteClientUrl": {
          "@odata.type": "microsoft.graph.externalLink",
          "href": "Href value"
        },
        "oneNoteWebUrl": {
          "@odata.type": "microsoft.graph.externalLink"
        }
      }
    }
  ]
}
```

