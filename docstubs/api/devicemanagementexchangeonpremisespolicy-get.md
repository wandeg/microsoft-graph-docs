---
title: "Get deviceManagementExchangeOnPremisesPolicy"
description: "Read properties and relationships of the deviceManagementExchangeOnPremisesPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementExchangeOnPremisesPolicy

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.

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
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementexchangeonpremisespolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 723

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "c1178ec7-8ec7-c117-c78e-17c1c78e17c1",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "String",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "String"
        },
        "accessLevel": "String"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
      }
    ]
  }
}
```

