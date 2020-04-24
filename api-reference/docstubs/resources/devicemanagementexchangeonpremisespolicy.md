---
title: "deviceManagementExchangeOnPremisesPolicy resource type"
description: "Singleton entity which represents the Exchange OnPremises policy configured for a tenant."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementExchangeOnPremisesPolicy resource type


Namespace: microsoft.graph

Singleton entity which represents the Exchange OnPremises policy configured for a tenant.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementExchangeOnPremisesPolicy](../api/devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Read the properties and relationships of a [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[Update deviceManagementExchangeOnPremisesPolicy](../api/devicemanagementexchangeonpremisespolicy-update.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md)|Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) object.|
|[List conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-list-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) collection|Get the onPremisesConditionalAccessSettings from the conditionalAccessSettings navigation property.|
|[Create conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-post-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Create a new conditionalAccessSettings object.|
|[Delete conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-delete-conditionalaccesssettings.md)|None|Delete a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Update conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-update-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Update the properties of a conditionalAccessSettings object.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Read the properties and relationships of an [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRules|[deviceManagementExchangeAccessRule](../resources/devicemanagementexchangeaccessrule.md) collection|The list of device access rules in Exchange. The access rules apply globally to the entire Exchange organization|
|defaultAccessLevel|deviceManagementExchangeAccessLevel|Default access state in Exchange. This rule applies globally to the entire Exchange organization. Possible values are: `none`, `allow`, `block`, `quarantine`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|knownDeviceClasses|[deviceManagementExchangeDeviceClass](../resources/devicemanagementexchangedeviceclass.md) collection|The list of device classes known to Exchange|
|notificationContent|Binary|Notification text that will be sent to users quarantined by this policy. This is UTF8 encoded byte array HTML.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|The Exchange on premises conditional access settings. On premises conditional access will require devices to be both enrolled and compliant for mail access|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
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

