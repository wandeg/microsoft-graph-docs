---
title: "deviceCompliancePolicyPolicySetItem resource type"
description: "A class containing the properties used for device compliance policy PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceCompliancePolicyPolicySetItem resource type

A class containing the properties used for device compliance policy PolicySetItem.


Inherits from [policySetItem](../resources/policySetItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceCompliancePolicyPolicySetItems](../api/devicecompliancepolicypolicysetitem-list.md)|[deviceCompliancePolicyPolicySetItem](../resources/deviceCompliancePolicyPolicySetItem.md) collection|List properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/devicecompliancepolicypolicysetitem.md) objects.|
|[Get deviceCompliancePolicyPolicySetItem](../api/devicecompliancepolicypolicysetitem-get.md)|[deviceCompliancePolicyPolicySetItem](../resources/deviceCompliancePolicyPolicySetItem.md)|Read properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/devicecompliancepolicypolicysetitem.md) object.|
|[Create deviceCompliancePolicyPolicySetItem](../api/devicecompliancepolicypolicysetitem-create.md)|[deviceCompliancePolicyPolicySetItem](../resources/deviceCompliancePolicyPolicySetItem.md)|Create a new [deviceCompliancePolicyPolicySetItem](../resources/devicecompliancepolicypolicysetitem.md) object.|
|[Delete deviceCompliancePolicyPolicySetItem](../api/devicecompliancepolicypolicysetitem-delete.md)|None|Deletes a [deviceCompliancePolicyPolicySetItem](../resources/devicecompliancepolicypolicysetitem.md).|
|[Update deviceCompliancePolicyPolicySetItem](../api/devicecompliancepolicypolicysetitem-update.md)|[deviceCompliancePolicyPolicySetItem](../resources/deviceCompliancePolicyPolicySetItem.md)|Update the properties of a [deviceCompliancePolicyPolicySetItem](../resources/devicecompliancepolicypolicysetitem.md) object.|

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
  "@odata.type": "microsoft.graph.deviceCompliancePolicyPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
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

