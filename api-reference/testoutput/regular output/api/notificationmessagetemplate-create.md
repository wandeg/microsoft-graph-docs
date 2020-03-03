---
title: "Create notificationMessageTemplate"
description: "Create a new notificationMessageTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create notificationMessageTemplate

Namespace: microsoft.graph

Create a new [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.

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
POST /deviceManagement/notificationMessageTemplates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.

The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/notificationmessagetemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Display name for the Notification Message Template.|
|defaultLocale|String|The default locale to fallback onto when the requested locale is not available.|
|brandingOptions|Enumeration|The Message Template Branding Options. Branding is defined in the Intune Admin Console. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|



## Response
If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_notificationmessagetemplate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notificationmessagetemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "4106bfab-bfab-4106-abbf-0641abbf0641",
  "lastModifiedDateTime": "2017-01-01T00:00:08.5199759+03:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String"
}
```

