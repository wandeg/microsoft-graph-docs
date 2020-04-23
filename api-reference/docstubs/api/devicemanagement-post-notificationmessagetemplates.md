---
title: "Create notificationMessageTemplates"
description: "Create a new notificationMessageTemplates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create notificationMessageTemplates

Namespace: microsoft.graph

Create a new notificationMessageTemplates object.

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
POST /deviceManagement/notificationMessageTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.

The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/notificationmessagetemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Display name for the Notification Message Template.|
|defaultLocale|String|The default locale to fallback onto when the requested locale is not available.|
|brandingOptions|notificationTemplateBrandingOptions|The Message Template Branding Options. Branding is defined in the Intune Admin Console. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|



## Response
If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_notificationmessagetemplate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
Content-Type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notificationmessagetemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "3fe81dce-1dce-3fe8-ce1d-e83fce1de83f",
  "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String"
}
```

