---
title: "createInstance"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createInstance

Namespace: microsoft.graph



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
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|description|String||
|settingsDelta|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection||
|roleScopeTagIds|String collection||



## Response
If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/devicemanagementintent.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "devicemanagementtemplate_createinstance"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 398

{
  "displayName": "Display Name value",
  "description": "Description value",
  "settingsDelta": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "da3bef94-ef94-da3b-94ef-3bda94ef3bda",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementintent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "85b798a0-98a0-85b7-a098-b785a098b785",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```

