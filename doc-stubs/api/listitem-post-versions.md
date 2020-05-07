---
title: "Create versions"
description: "Create a new versions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create versions

Namespace: microsoft.graph

Create a new versions object.

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
POST /workbooks/{workbooksId}/activities/{itemActivityOLDId}/listItem/versions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [listItemVersion](../resources/listitemversion.md) object.

The following table shows the properties that are required when you create the [listItemVersion](../resources/listitemversion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|



## Response

If successful, this method returns a `201 Created` response code and a [listItemVersion](../resources/listitemversion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_listitemversion_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/activities/{itemActivityOLDId}/listItem/versions
Content-Type: application/json
Content-length: 138

{
  "@odata.type": "#microsoft.graph.listItemVersion",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.listitemversion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.listItemVersion",
  "id": "992b473d-473d-992b-3d47-2b993d472b99",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  }
}
```

