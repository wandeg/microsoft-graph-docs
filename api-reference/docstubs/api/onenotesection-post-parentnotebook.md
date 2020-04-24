---
title: "Create parentNotebook"
description: "Create a new parentNotebook object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create parentNotebook

Namespace: microsoft.graph

Create a new parentNotebook object.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentNotebook
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [notebook](../resources/notebook.md) object.

The following table shows the properties that are required when you create the [notebook](../resources/notebook.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|isDefault|Boolean|**TODO: Add Description**|
|userRole|onenoteUserRole|**TODO: Add Description**. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|
|isShared|Boolean|**TODO: Add Description**|
|sectionsUrl|String|**TODO: Add Description**|
|sectionGroupsUrl|String|**TODO: Add Description**|
|links|[notebookLinks](../resources/notebooklinks.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [notebook](../resources/notebook.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentNotebook
Content-Type: application/json
Content-length: 899

{
  "@odata.type": "#microsoft.graph.notebook",
  "self": "Self value",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
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
```

