---
title: "iosLobAppProvisioningConfigurationPolicySetItem resource type"
description: "A class containing the properties used for iOS lob app provisioning configuration PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosLobAppProvisioningConfigurationPolicySetItem resource type


Namespace: microsoft.graph

A class containing the properties used for iOS lob app provisioning configuration PolicySetItem.


Inherits from [policySetItem](../resources/policysetitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosLobAppProvisioningConfigurationPolicySetItems](../api/ioslobappprovisioningconfigurationpolicysetitem-list.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md) collection|List properties and relationships of the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md) objects.|
|[Get iosLobAppProvisioningConfigurationPolicySetItem](../api/ioslobappprovisioningconfigurationpolicysetitem-get.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md)|Read properties and relationships of the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md) object.|
|[Create iosLobAppProvisioningConfigurationPolicySetItem](../api/ioslobappprovisioningconfigurationpolicysetitem-create.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md)|Create a new [iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md) object.|
|[Delete iosLobAppProvisioningConfigurationPolicySetItem](../api/ioslobappprovisioningconfigurationpolicysetitem-delete.md)|None|Deletes a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md).|
|[Update iosLobAppProvisioningConfigurationPolicySetItem](../api/ioslobappprovisioningconfigurationpolicysetitem-update.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md)|Update the properties of a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/ioslobappprovisioningconfigurationpolicysetitem.md) object.|

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
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
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

