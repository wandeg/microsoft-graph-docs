---
title: "Update groupSettingTemplate"
description: "Update the properties of a groupSettingTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupSettingTemplate

Namespace: microsoft.graph

Update the properties of a [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

The following table shows the properties that are required when you create the [groupSettingTemplate](../resources/groupsettingtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String||
|description|String||
|values|[settingTemplateValue](../resources/settingtemplatevalue.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_groupsettingtemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groupSettingTemplates/{groupSettingTemplatesId}
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "deletedDateTime": "2016-12-31T23:59:15.8984066+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 449

{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "id": "7fb47288-7288-7fb4-8872-b47f8872b47f",
  "deletedDateTime": "2016-12-31T23:59:15.8984066+03:00",
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

