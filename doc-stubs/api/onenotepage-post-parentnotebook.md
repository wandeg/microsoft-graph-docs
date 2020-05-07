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
POST /users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentNotebook
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
POST https://graph.microsoft.com/beta/users/{usersId}/onenote/notebooks/{notebookId}/sections/{onenoteSectionId}/pages/{onenotePageId}/parentNotebook
Content-Type: application/json
Content-length: 384

{
  "@odata.type": "#microsoft.graph.notebook",
  "self": "String",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "isDefault": "Boolean",
  "userRole": "String",
  "isShared": "Boolean",
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks"
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
  "id": "cd1fc1a5-c1a5-cd1f-a5c1-1fcda5c11fcd",
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
  "userRole": "String",
  "isShared": "Boolean",
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks"
  }
}
```

