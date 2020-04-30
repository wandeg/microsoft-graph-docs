---
title: "Update versions"
description: "Update the properties of a versions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update versions

Namespace: microsoft.graph

Update the properties of a versions object.

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
PATCH /workbooks/{workbooksId}/versions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [driveItemVersion](../resources/driveitemversion.md) object.

The following table shows the properties that are required when you create the [driveItemVersion](../resources/driveitemversion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description** Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|content|Stream|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [driveItemVersion](../resources/driveitemversion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_versions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbooks/{workbooksId}/versions
Content-Type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "content": "Stream",
  "size": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "id": "3b4e9196-9196-3b4e-9691-4e3b96914e3b",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "content": "Stream",
  "size": "Integer"
}
```

