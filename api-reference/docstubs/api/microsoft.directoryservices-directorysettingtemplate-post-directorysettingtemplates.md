---
title: "Create directorySettingTemplate"
description: "Create a new directorySettingTemplate object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create directorySettingTemplate

Namespace: Microsoft.DirectoryServices

Create a new [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) object.

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
POST /directorySettingTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) object.

The following table shows the properties that are required when you create the [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|values|[settingTemplateValue](../resources/microsoft.directoryservices-settingtemplatevalue.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directorysettingtemplate_from_directorysettingtemplates"
}
-->
``` http
POST https://graph.microsoft.com/changelog/directorySettingTemplates
Content-Type: application/json
Content-length: 428

{
  "@odata.type": "#Microsoft.DirectoryServices.directorySettingTemplate",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "values": [
    {
      "@odata.type": "Microsoft.DirectoryServices.settingTemplateValue",
      "name": "Name value",
      "type": "Type value",
      "defaultValue": "Default Value value"
    }
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.directorysettingtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.directorySettingTemplate",
  "id": "843c296e-296e-843c-6e29-3c846e293c84",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "values": [
    {
      "@odata.type": "Microsoft.DirectoryServices.settingTemplateValue",
      "name": "Name value",
      "type": "Type value",
      "defaultValue": "Default Value value"
    }
  ]
}
```

