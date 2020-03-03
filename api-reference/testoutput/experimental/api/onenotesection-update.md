---
title: "Update onenoteSection"
description: "Update the properties of a onenoteSection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onenoteSection

Update the properties of a [onenoteSection](../resources/onenotesection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/sections/{onenoteSectionId}
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentSection
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/parentSectionGroup/sections/{onenoteSectionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [onenoteSection](../resources/onenoteSection.md) object.

The following table shows the properties that are required when you create the [onenoteSection](../resources/onenotesection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteEntityBaseModel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|isDefault|Boolean||
|links|[sectionLinks](../resources/sectionLinks.md)||
|pagesUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [onenoteSection](../resources/onenotesection.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onenotesection"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/sites/{siteId}/onenote/sections/{onenoteSectionId}
Content-type: application/json
Content-length: 788

{
  "@odata.type": "#microsoft.graph.onenoteSection",
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
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "Href value"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "pagesUrl": "https://example.com/pagesUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1039

{
  "@odata.type": "#microsoft.graph.onenoteSection",
  "id": "ca9c914a-914a-ca9c-4a91-9cca4a919cca",
  "self": "Self value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "isDefault": true,
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "Href value"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "pagesUrl": "https://example.com/pagesUrl/"
}
```

