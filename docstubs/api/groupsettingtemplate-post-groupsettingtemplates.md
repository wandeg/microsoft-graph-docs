---
title: "Create groupSettingTemplate"
description: "Create a new groupSettingTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create groupSettingTemplate

Namespace: microsoft.graph

Create a new [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

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
POST /groupSettingTemplates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_groupsettingtemplate_from_groupsettingtemplates"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groupSettingTemplates
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "deletedDateTime": "2017-01-01T00:00:51.5607674+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.groupsettingtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 449

{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "id": "1a34eb3b-eb3b-1a34-3beb-341a3beb341a",
  "deletedDateTime": "2017-01-01T00:00:51.5607674+03:00",
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

