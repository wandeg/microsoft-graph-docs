---
title: "List exchangeOnPremisesPolicies"
description: "Get the deviceManagementExchangeOnPremisesPolicies from the exchangeOnPremisesPolicies navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List exchangeOnPremisesPolicies

Get the deviceManagementExchangeOnPremisesPolicies from the exchangeOnPremisesPolicies navigation property.

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
GET /deviceManagement/exchangeOnPremisesPolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementexchangeonpremisespolicy"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/deviceManagement/exchangeOnPremisesPolicies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementexchangeonpremisespolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
      "id": "5d1b1915-1915-5d1b-1519-1b5d15191b5d",
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
  ]
}
```

