---
title: "Create referenceAttachment"
description: "Create a new referenceAttachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create referenceAttachment

Namespace: microsoft.graph

Create a new [referenceAttachment](../resources/referenceattachment.md) object.

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
POST ** Collection URI for microsoft.graph.referenceAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [referenceAttachment](../resources/referenceattachment.md) object.

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
If successful, this method returns a `201 Created` response code and a [referenceAttachment](../resources/referenceattachment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_referenceattachment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.referenceAttachment not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceattachment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 509

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "eb77e7aa-e7aa-eb77-aae7-77ebaae777eb",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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

