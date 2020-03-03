---
title: "managedAppProtectionPolicySetItem resource type"
description: "A class containing the properties used for managed app protection PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAppProtectionPolicySetItem resource type

A class containing the properties used for managed app protection PolicySetItem.


Inherits from [policySetItem](../resources/policySetItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppProtectionPolicySetItems](../api/managedappprotectionpolicysetitem-list.md)|[managedAppProtectionPolicySetItem](../resources/managedAppProtectionPolicySetItem.md) collection|List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md) objects.|
|[Get managedAppProtectionPolicySetItem](../api/managedappprotectionpolicysetitem-get.md)|[managedAppProtectionPolicySetItem](../resources/managedAppProtectionPolicySetItem.md)|Read properties and relationships of the [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md) object.|
|[Create managedAppProtectionPolicySetItem](../api/managedappprotectionpolicysetitem-create.md)|[managedAppProtectionPolicySetItem](../resources/managedAppProtectionPolicySetItem.md)|Create a new [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md) object.|
|[Delete managedAppProtectionPolicySetItem](../api/managedappprotectionpolicysetitem-delete.md)|None|Deletes a [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md).|
|[Update managedAppProtectionPolicySetItem](../api/managedappprotectionpolicysetitem-update.md)|[managedAppProtectionPolicySetItem](../resources/managedAppProtectionPolicySetItem.md)|Update the properties of a [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md) object.|

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
|targetedAppManagementLevels|String|TargetedAppManagementLevels of the ManagedAppPolicySetItem.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtectionPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
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
  ],
  "targetedAppManagementLevels": "String"
}
```

