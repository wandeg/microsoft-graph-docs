---
title: "Add files"
description: "Add files by posting to the files collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add files

Add files by posting to the files collection.

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
POST /agreements/{agreementsId}/files/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the agreementFile object.

The following table shows the properties that are required when you create the agreementFile.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|language|String||
|fileName|String||
|fileData|[agreementFileData](../resources/agreementFileData.md)||
|isDefault|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [agreementFile](../resources/agreementfile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_agreementfile_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/agreements/{agreementsId}/files
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.agreementFile",
  "language": "Language value",
  "fileName": "File Name value",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData",
    "data": "ZGF0YQ=="
  },
  "isDefault": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementfile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.agreementFile",
  "id": "1ad53af8-3af8-1ad5-f83a-d51af83ad51a",
  "language": "Language value",
  "fileName": "File Name value",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData",
    "data": "ZGF0YQ=="
  },
  "isDefault": true
}
```

