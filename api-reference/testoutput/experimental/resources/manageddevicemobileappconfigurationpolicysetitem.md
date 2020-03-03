---
title: "managedDeviceMobileAppConfigurationPolicySetItem resource type"
description: "A class containing the properties used for managed device mobile app configuration PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedDeviceMobileAppConfigurationPolicySetItem resource type

A class containing the properties used for managed device mobile app configuration PolicySetItem.


Inherits from [policySetItem](../resources/policySetItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedDeviceMobileAppConfigurationPolicySetItems](../api/manageddevicemobileappconfigurationpolicysetitem-list.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/managedDeviceMobileAppConfigurationPolicySetItem.md) collection|List properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) objects.|
|[Get managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-get.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/managedDeviceMobileAppConfigurationPolicySetItem.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) object.|
|[Create managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-create.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/managedDeviceMobileAppConfigurationPolicySetItem.md)|Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) object.|
|[Delete managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-delete.md)|None|Deletes a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md).|
|[Update managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-update.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/managedDeviceMobileAppConfigurationPolicySetItem.md)|Update the properties of a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Creation time of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|displayName|String|DisplayName of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|errorCode|Enumeration|Error code if any occured. Inherited from [policySetItem](../resources/policySetItem.md). Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment Inherited from [policySetItem](../resources/policySetItem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|itemType|String|policySetType of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|payloadId|String|PayloadId of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|status|Enumeration|Status of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md). Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
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

