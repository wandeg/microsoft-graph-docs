---
title: "Create fileAttachment"
description: "Create a new fileAttachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create fileAttachment

Create a new [fileAttachment](../resources/fileattachment.md) object.

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
POST ** Collection URI for microsoft.graph.fileAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the fileAttachment object.

The following table shows the properties that are required when you create the fileAttachment.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [attachment](../resources/attachment.md)|
|name|String| Inherited from [attachment](../resources/attachment.md)|
|contentType|String| Inherited from [attachment](../resources/attachment.md)|
|size|Int32| Inherited from [attachment](../resources/attachment.md)|
|isInline|Boolean| Inherited from [attachment](../resources/attachment.md)|
|contentId|String||
|contentLocation|String||
|contentBytes|Binary||



## Response
If successful, this method returns a `201 Created` response code and a [fileAttachment](../resources/fileattachment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_fileattachment_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.fileAttachment not found
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true,
  "contentId": "Content Id value",
  "contentLocation": "Content Location value",
  "contentBytes": "Y29udGVudEJ5dGVz"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileattachment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 392

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "id": "b4bf742a-742a-b4bf-2a74-bfb42a74bfb4",
  "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true,
  "contentId": "Content Id value",
  "contentLocation": "Content Location value",
  "contentBytes": "Y29udGVudEJ5dGVz"
}
```

