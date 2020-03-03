---
title: "List androidManagedStoreAppConfigurationSchemas"
description: "List properties and relationships of the androidManagedStoreAppConfigurationSchema objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List androidManagedStoreAppConfigurationSchemas

Namespace: microsoft.graph

List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) objects.

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
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androidmanagedstoreappconfigurationschema"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.androidmanagedstoreappconfigurationschema)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1191

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
      "id": "17339224-9224-1733-2492-331724923317",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
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
      ],
      "nestedSchemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
        }
      ]
    }
  ]
}
```

