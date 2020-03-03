---
title: "Add notebooks"
description: "Add notebooks by posting to the notebooks collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add notebooks

Add notebooks by posting to the notebooks collection.

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
POST /me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the notebook object.

The following table shows the properties that are required when you create the notebook.

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
|userRole|Enumeration|. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|
|isShared|Boolean||
|sectionsUrl|String||
|sectionGroupsUrl|String||
|links|[notebookLinks](../resources/notebookLinks.md)||



## Response
If successful, this method returns a `201 Created` response code and a [notebook](../resources/notebook.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/sites/{siteId}/onenote/notebooks
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.notebook",
  "id": "a1c6ab37-ab37-a1c6-37ab-c6a137abc6a1",
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

