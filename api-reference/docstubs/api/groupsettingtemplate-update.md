---
title: "Update groupSettingTemplate"
description: "Update the properties of a groupSettingTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupSettingTemplate

Namespace: microsoft.graph

Update the properties of a [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

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
PATCH /groupSettingTemplates/{groupSettingTemplatesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

The following table shows the properties that are required when you create the [groupSettingTemplate](../resources/groupsettingtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|values|[settingTemplateValue](../resources/settingtemplatevalue.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_groupsettingtemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groupSettingTemplates/{groupSettingTemplatesId}
Content-Type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "deletedDateTime": "2016-12-31T23:58:36.4652914+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingTemplateValue",
      "name": "Name value",
      "type": "Type value",
      "defaultValue": "Default Value value"
    }
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
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "id": "7aea353a-353a-7aea-3a35-ea7a3a35ea7a",
  "deletedDateTime": "2016-12-31T23:58:36.4652914+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingTemplateValue",
      "name": "Name value",
      "type": "Type value",
      "defaultValue": "Default Value value"
    }
  ]
}
```

