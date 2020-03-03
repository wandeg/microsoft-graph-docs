---
title: "managedDeviceMobileAppConfigurationPolicySetItem resource type"
description: "A class containing the properties used for managed device mobile app configuration PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceMobileAppConfigurationPolicySetItem resource type


Namespace: microsoft.graph

A class containing the properties used for managed device mobile app configuration PolicySetItem.


Inherits from [policySetItem](../resources/policysetitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedDeviceMobileAppConfigurationPolicySetItems](../api/manageddevicemobileappconfigurationpolicysetitem-list.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) collection|List properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) objects.|
|[Get managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-get.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) object.|
|[Create managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-create.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md)|Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) object.|
|[Delete managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-delete.md)|None|Deletes a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md).|
|[Update managedDeviceMobileAppConfigurationPolicySetItem](../api/manageddevicemobileappconfigurationpolicysetitem-update.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md)|Update the properties of a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/manageddevicemobileappconfigurationpolicysetitem.md) object.|

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

