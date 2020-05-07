---
title: "Update mentions"
description: "Update the properties of a mentions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update mentions

Namespace: microsoft.graph

Update the properties of a mentions object.

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
PATCH /users/{usersId}/messages/{messageId}/mentions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mention](../resources/mention.md) object.

The following table shows the properties that are required when you create the [mention](../resources/mention.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|mentioned|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|mentionText|String|**TODO: Add Description**|
|clientReference|String|**TODO: Add Description**|
|createdBy|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|serverCreatedDateTime|DateTimeOffset|**TODO: Add Description**|
|deepLink|String|**TODO: Add Description**|
|application|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [mention](../resources/mention.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_mentions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/messages/{messageId}/mentions
Content-Type: application/json
Content-length: 362

{
  "@odata.type": "#microsoft.graph.mention",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "mentionText": "String",
  "clientReference": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "serverCreatedDateTime": "String (timestamp)",
  "deepLink": "String",
  "application": "String"
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
  "@odata.type": "#microsoft.graph.mention",
  "id": "29373160-3160-2937-6031-372960313729",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "mentionText": "String",
  "clientReference": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "createdDateTime": "String (timestamp)",
  "serverCreatedDateTime": "String (timestamp)",
  "deepLink": "String",
  "application": "String"
}
```

