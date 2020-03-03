---
title: "Update referenceAttachment"
description: "Update the properties of a referenceAttachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update referenceAttachment

Update the properties of a [referenceAttachment](../resources/referenceattachment.md) object.

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
PATCH ** Entity URI for microsoft.graph.referenceAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [referenceAttachment](../resources/referenceAttachment.md) object.

The following table shows the properties that are required when you create the [referenceAttachment](../resources/referenceattachment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [attachment](../resources/attachment.md)|
|name|String| Inherited from [attachment](../resources/attachment.md)|
|contentType|String| Inherited from [attachment](../resources/attachment.md)|
|size|Int32| Inherited from [attachment](../resources/attachment.md)|
|isInline|Boolean| Inherited from [attachment](../resources/attachment.md)|
|sourceUrl|String||
|providerType|Enumeration|. Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.|
|thumbnailUrl|String||
|previewUrl|String||
|permission|Enumeration|. Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.|
|isFolder|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [referenceAttachment](../resources/referenceattachment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_referenceattachment"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.referenceAttachment not found
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true,
  "sourceUrl": "https://example.com/sourceUrl/",
  "providerType": "String",
  "thumbnailUrl": "https://example.com/thumbnailUrl/",
  "previewUrl": "https://example.com/previewUrl/",
  "permission": "String",
  "isFolder": true
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
Content-Length: 509

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "9895a6d5-a6d5-9895-d5a6-9598d5a69598",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true,
  "sourceUrl": "https://example.com/sourceUrl/",
  "providerType": "String",
  "thumbnailUrl": "https://example.com/thumbnailUrl/",
  "previewUrl": "https://example.com/previewUrl/",
  "permission": "String",
  "isFolder": true
}
```

