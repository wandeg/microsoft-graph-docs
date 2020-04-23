---
title: "Update managedEBooks"
description: "Update the properties of a managedEBooks object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedEBooks

Namespace: microsoft.graph

Update the properties of a managedEBooks object.

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
PATCH /deviceAppManagement/managedEBooks
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
If successful, this method returns a `200 OK` response code and an updated [managedEBook](../resources/managedebook.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managedebooks"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-Type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.managedEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2017-01-01T00:02:44.4432167+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "99622f8d-2f8d-9962-8d2f-62998d2f6299",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2017-01-01T00:02:44.4432167+03:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
  "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
}
```

