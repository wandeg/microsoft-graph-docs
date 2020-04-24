---
title: "Update notificationMessageTemplates"
description: "Update the properties of a notificationMessageTemplates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update notificationMessageTemplates

Namespace: microsoft.graph

Update the properties of a notificationMessageTemplates object.

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
PATCH /deviceManagement/notificationMessageTemplates
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
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|



## Response
If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_notificationmessagetemplates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
Content-Type: application/json
Content-length: 247

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
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
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "9141dc3d-dc3d-9141-3ddc-41913ddc4191",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

