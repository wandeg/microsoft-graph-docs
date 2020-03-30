---
title: "Add androidForWorkAppConfigurationSchemas"
description: "Add androidForWorkAppConfigurationSchemas by posting to the androidForWorkAppConfigurationSchemas collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add androidForWorkAppConfigurationSchemas

Namespace: microsoft.graph

Add androidForWorkAppConfigurationSchemas by posting to the androidForWorkAppConfigurationSchemas collection.

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
POST /deviceManagement/androidForWorkAppConfigurationSchemas/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.

The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|exampleJson|Binary||
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/androidforworkappconfigurationschemaitem.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_androidforworkappconfigurationschema_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
Content-type: application/json
Content-length: 794

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidforworkappconfigurationschema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 843

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "7d352dc6-2dc6-7d35-c62d-357dc62d357d",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

