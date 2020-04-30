---
title: "driveItem: restore"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# restore

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /workbooks/{workbooksId}/restore
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_restore"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/restore

Content-Type: application/json
Content-length: 106

{
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "name": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveitem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.driveItem",
    "id": "String (identifier)",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "eTag": "String",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "name": "String",
    "parentReference": {
      "@odata.type": "microsoft.graph.itemReference"
    },
    "webUrl": "String",
    "audio": {
      "@odata.type": "microsoft.graph.audio"
    },
    "bundle": {
      "@odata.type": "microsoft.graph.bundle"
    },
    "content": "Stream",
    "cTag": "String",
    "deleted": {
      "@odata.type": "microsoft.graph.deleted"
    },
    "file": {
      "@odata.type": "microsoft.graph.file"
    },
    "fileSystemInfo": {
      "@odata.type": "microsoft.graph.fileSystemInfo"
    },
    "folder": {
      "@odata.type": "microsoft.graph.folder"
    },
    "image": {
      "@odata.type": "microsoft.graph.image"
    },
    "location": {
      "@odata.type": "microsoft.graph.geoCoordinates"
    },
    "package": {
      "@odata.type": "microsoft.graph.package"
    },
    "pendingOperations": {
      "@odata.type": "microsoft.graph.pendingOperations"
    },
    "photo": {
      "@odata.type": "microsoft.graph.photo"
    },
    "publication": {
      "@odata.type": "microsoft.graph.publicationFacet"
    },
    "remoteItem": {
      "@odata.type": "microsoft.graph.remoteItem"
    },
    "root": {
      "@odata.type": "microsoft.graph.root"
    },
    "searchResult": {
      "@odata.type": "microsoft.graph.searchResult"
    },
    "shared": {
      "@odata.type": "microsoft.graph.shared"
    },
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds"
    },
    "size": "Integer",
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "video": {
      "@odata.type": "microsoft.graph.video"
    },
    "webDavUrl": "String"
  }
}
```

