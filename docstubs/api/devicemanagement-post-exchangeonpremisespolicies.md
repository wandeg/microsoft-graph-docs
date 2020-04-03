---
title: "Add exchangeOnPremisesPolicies"
description: "Add exchangeOnPremisesPolicies by posting to the exchangeOnPremisesPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add exchangeOnPremisesPolicies

Namespace: microsoft.graph

Add exchangeOnPremisesPolicies by posting to the exchangeOnPremisesPolicies collection.

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
POST /deviceManagement/exchangeOnPremisesPolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.

The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|notificationContent|Binary||
|defaultAccessLevel|Enumeration| Possible values are: `none`, `allow`, `block`, `quarantine`.|
|accessRules|[deviceManagementExchangeAccessRule](../resources/devicemanagementexchangeaccessrule.md) collection||
|knownDeviceClasses|[deviceManagementExchangeDeviceClass](../resources/devicemanagementexchangedeviceclass.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementexchangeonpremisespolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicies
Content-type: application/json
Content-length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementexchangeonpremisespolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 664

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "eb1f8855-8855-eb1f-5588-1feb55881feb",
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
```

