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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedEBook](../resources/intune-managedebook.md) object.

The following table shows the properties that are required when you create the [managedEBook](../resources/intune-managedebook.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|publishedDateTime|DateTimeOffset|**TODO: Add Description**|
|largeCover|[mimeContent](../resources/intune-mimecontent.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|informationUrl|String|**TODO: Add Description**|
|privacyInformationUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedEBook](../resources/intune-managedebook.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_managedebooks"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-Type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.managedEBook",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "informationUrl": "String",
  "privacyInformationUrl": "String"
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
  "id": "f246cdc7-cdc7-f246-c7cd-46f2c7cd46f2",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```

