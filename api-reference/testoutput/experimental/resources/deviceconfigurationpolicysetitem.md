---
title: "deviceConfigurationPolicySetItem resource type"
description: "A class containing the properties used for device configuration PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationPolicySetItem resource type


Namespace: microsoft.graph

A class containing the properties used for device configuration PolicySetItem.


Inherits from [policySetItem](../resources/policysetitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceConfigurationPolicySetItems](../api/deviceconfigurationpolicysetitem-list.md)|[deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md) collection|List properties and relationships of the [deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md) objects.|
|[Get deviceConfigurationPolicySetItem](../api/deviceconfigurationpolicysetitem-get.md)|[deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md)|Read properties and relationships of the [deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md) object.|
|[Create deviceConfigurationPolicySetItem](../api/deviceconfigurationpolicysetitem-create.md)|[deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md)|Create a new [deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md) object.|
|[Delete deviceConfigurationPolicySetItem](../api/deviceconfigurationpolicysetitem-delete.md)|None|Deletes a [deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md).|
|[Update deviceConfigurationPolicySetItem](../api/deviceconfigurationpolicysetitem-update.md)|[deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md)|Update the properties of a [deviceConfigurationPolicySetItem](../resources/deviceconfigurationpolicysetitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Creation time of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md)|
|displayName|String|DisplayName of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md)|
|errorCode|Enumeration|Error code if any occured. Inherited from [policySetItem](../resources/policysetitem.md). Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment Inherited from [policySetItem](../resources/policysetitem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|itemType|String|policySetType of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md)|
|payloadId|String|PayloadId of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md)|
|status|Enumeration|Status of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md). Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```

