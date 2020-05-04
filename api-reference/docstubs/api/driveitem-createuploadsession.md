---
title: "driveItem: createUploadSession"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# createUploadSession

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
POST /drive/root/createUploadSession
POST /drives/{drivesId}/root/createUploadSession
POST /shares/{sharesId}/root/createUploadSession
POST /workbooks/{workbooksId}/createUploadSession
POST /drive/items/{driveItemId}/createUploadSession
POST /shares/{sharesId}/driveItem/createUploadSession
POST /drive/bundles/{driveItemId}/createUploadSession
POST /drive/special/{driveItemId}/createUploadSession
POST /drive/following/{driveItemId}/createUploadSession
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|item|[driveItemUploadableProperties](../resources/driveitemuploadableproperties.md)|**TODO: Add Description**|
|deferCommit|Boolean|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [uploadSession](../resources/uploadsession.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/root/createUploadSession

Content-Type: application/json
Content-length: 134

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "fileSize": 8
  },
  "deferCommit": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadsession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.graph.uploadSession"
  }
}
```

