---
title: "onPremisesConditionalAccessSettings resource type"
description: "Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onPremisesConditionalAccessSettings resource type

Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onPremisesConditionalAccessSettingses](../api/onpremisesconditionalaccesssettings-list.md)|[onPremisesConditionalAccessSettings](../resources/onPremisesConditionalAccessSettings.md) collection|List properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) objects.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onPremisesConditionalAccessSettings.md)|Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Create onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-create.md)|[onPremisesConditionalAccessSettings](../resources/onPremisesConditionalAccessSettings.md)|Create a new [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Delete onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-delete.md)|None|Deletes a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md).|
|[Update onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/onPremisesConditionalAccessSettings.md)|Update the properties of a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|enabled|Boolean|Indicates if on premises conditional access is enabled for this organization|
|excludedGroups|Guid collection|User groups that will be exempt by on premises conditional access. All users in these groups will be exempt from the conditional access policy.|
|id|String| Inherited from [entity](../resources/entity.md)|
|includedGroups|Guid collection|User groups that will be targeted by on premises conditional access. All users in these groups will be required to have mobile device managed and compliant for mail access.|
|overrideDefaultRule|Boolean|Override the default access rule when allowing a device to ensure access is granted.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```

