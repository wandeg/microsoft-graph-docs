---
title: "deviceManagementExchangeOnPremisesPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementExchangeOnPremisesPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-list-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) collection|Get the onPremisesConditionalAccessSettings from the conditionalAccessSettings navigation property.|
|[Create conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-post-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Create a new conditionalAccessSettings object.|
|[Delete conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-delete-conditionalaccesssettings.md)|None|Delete a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Update conditionalAccessSettings](../api/devicemanagementexchangeonpremisespolicy-update-conditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Update the properties of a conditionalAccessSettings object.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Read the properties and relationships of an [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRules|[deviceManagementExchangeAccessRule](../resources/devicemanagementexchangeaccessrule.md) collection|**TODO: Add Description**|
|defaultAccessLevel|deviceManagementExchangeAccessLevel|**TODO: Add Description**. Possible values are: `none`, `allow`, `block`, `quarantine`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|knownDeviceClasses|[deviceManagementExchangeDeviceClass](../resources/devicemanagementexchangedeviceclass.md) collection|**TODO: Add Description**|
|notificationContent|Binary|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "notificationContent": "Binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
    }
  ]
}
```

