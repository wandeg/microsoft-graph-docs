---
title: "deviceManagementScriptPolicySetItem resource type"
description: "A class containing the properties used for device management script PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementScriptPolicySetItem resource type

A class containing the properties used for device management script PolicySetItem.


Inherits from [policySetItem](../resources/policySetItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementScriptPolicySetItems](../api/devicemanagementscriptpolicysetitem-list.md)|[deviceManagementScriptPolicySetItem](../resources/deviceManagementScriptPolicySetItem.md) collection|List properties and relationships of the [deviceManagementScriptPolicySetItem](../resources/devicemanagementscriptpolicysetitem.md) objects.|
|[Get deviceManagementScriptPolicySetItem](../api/devicemanagementscriptpolicysetitem-get.md)|[deviceManagementScriptPolicySetItem](../resources/deviceManagementScriptPolicySetItem.md)|Read properties and relationships of the [deviceManagementScriptPolicySetItem](../resources/devicemanagementscriptpolicysetitem.md) object.|
|[Create deviceManagementScriptPolicySetItem](../api/devicemanagementscriptpolicysetitem-create.md)|[deviceManagementScriptPolicySetItem](../resources/deviceManagementScriptPolicySetItem.md)|Create a new [deviceManagementScriptPolicySetItem](../resources/devicemanagementscriptpolicysetitem.md) object.|
|[Delete deviceManagementScriptPolicySetItem](../api/devicemanagementscriptpolicysetitem-delete.md)|None|Deletes a [deviceManagementScriptPolicySetItem](../resources/devicemanagementscriptpolicysetitem.md).|
|[Update deviceManagementScriptPolicySetItem](../api/devicemanagementscriptpolicysetitem-update.md)|[deviceManagementScriptPolicySetItem](../resources/deviceManagementScriptPolicySetItem.md)|Update the properties of a [deviceManagementScriptPolicySetItem](../resources/devicemanagementscriptpolicysetitem.md) object.|

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
  "@odata.type": "microsoft.graph.deviceManagementScriptPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
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

