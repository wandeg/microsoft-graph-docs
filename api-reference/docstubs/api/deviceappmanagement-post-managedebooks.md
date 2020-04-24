---
title: "Create managedEBooks"
description: "Create a new managedEBooks object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedEBooks

Namespace: microsoft.graph

Create a new managedEBooks object.

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
POST /deviceAppManagement/managedEBooks
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [managedEBook](../resources/managedebook.md) object.

The following table shows the properties that are required when you create the [managedEBook](../resources/managedebook.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|Name of the eBook.|
|description|String|Description.|
|publisher|String|Publisher.|
|publishedDateTime|DateTimeOffset|The date and time when the eBook was published.|
|largeCover|[mimeContent](../resources/mimecontent.md)|Book cover.|
|createdDateTime|DateTimeOffset|The date and time when the eBook file was created.|
|lastModifiedDateTime|DateTimeOffset|The date and time when the eBook was last modified.|
|informationUrl|String|The more information Url.|
|privacyInformationUrl|String|The privacy statement Url.|



## Response
If successful, this method returns a `201 Created` response code and a [managedEBook](../resources/managedebook.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managedebook_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-Type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.managedEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:59:48.8283567+03:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedebook"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "acd7f115-f115-acd7-15f1-d7ac15f1d7ac",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:59:48.8283567+03:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
}
```

