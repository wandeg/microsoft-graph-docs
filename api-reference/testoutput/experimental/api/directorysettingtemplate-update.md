---
title: "Update directorySettingTemplate"
description: "Update the properties of a directorySettingTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directorySettingTemplate

Namespace: microsoft.graph

Update the properties of a [directorySettingTemplate](../resources/directorysettingtemplate.md) object.

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
PATCH /directorySettingTemplates/{directorySettingTemplatesId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [directorySettingTemplate](../resources/directorysettingtemplate.md) object.

The following table shows the properties that are required when you create the [directorySettingTemplate](../resources/directorysettingtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String||
|description|String||
|values|[settingTemplateValue](../resources/settingtemplatevalue.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directorysettingtemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/directorySettingTemplates/{directorySettingTemplatesId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.directorySettingTemplate",
  "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
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
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.directorySettingTemplate",
  "id": "dc9d1200-1200-dc9d-0012-9ddc00129ddc",
  "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
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

