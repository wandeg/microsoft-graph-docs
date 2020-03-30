---
title: "Add settingDefinitions"
description: "Add settingDefinitions by posting to the settingDefinitions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add settingDefinitions

Namespace: microsoft.graph

Add settingDefinitions by posting to the settingDefinitions collection.

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
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.

The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|valueType|Enumeration| Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|String||
|isTopLevel|Boolean||
|description|String||
|placeholderText|String||
|documentationUrl|String||
|keywords|String collection||
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection||
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementsettingdefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
Content-type: application/json
Content-length: 708

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "valueType": "String",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value"
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementsettingdefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 757

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "95829c3f-9c3f-9582-3f9c-82953f9c8295",
  "valueType": "String",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value"
    }
  ]
}
```

