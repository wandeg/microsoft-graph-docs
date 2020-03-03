---
title: "mobileAppPolicySetItem resource type"
description: "A class containing the properties used for mobile app PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mobileAppPolicySetItem resource type

A class containing the properties used for mobile app PolicySetItem.


Inherits from [policySetItem](../resources/policySetItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppPolicySetItems](../api/mobileapppolicysetitem-list.md)|[mobileAppPolicySetItem](../resources/mobileAppPolicySetItem.md) collection|List properties and relationships of the [mobileAppPolicySetItem](../resources/mobileapppolicysetitem.md) objects.|
|[Get mobileAppPolicySetItem](../api/mobileapppolicysetitem-get.md)|[mobileAppPolicySetItem](../resources/mobileAppPolicySetItem.md)|Read properties and relationships of the [mobileAppPolicySetItem](../resources/mobileapppolicysetitem.md) object.|
|[Create mobileAppPolicySetItem](../api/mobileapppolicysetitem-create.md)|[mobileAppPolicySetItem](../resources/mobileAppPolicySetItem.md)|Create a new [mobileAppPolicySetItem](../resources/mobileapppolicysetitem.md) object.|
|[Delete mobileAppPolicySetItem](../api/mobileapppolicysetitem-delete.md)|None|Deletes a [mobileAppPolicySetItem](../resources/mobileapppolicysetitem.md).|
|[Update mobileAppPolicySetItem](../api/mobileapppolicysetitem-update.md)|[mobileAppPolicySetItem](../resources/mobileAppPolicySetItem.md)|Update the properties of a [mobileAppPolicySetItem](../resources/mobileapppolicysetitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Creation time of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|displayName|String|DisplayName of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|errorCode|Enumeration|Error code if any occured. Inherited from [policySetItem](../resources/policySetItem.md). Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment Inherited from [policySetItem](../resources/policySetItem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|intent|Enumeration|Install intent of the MobileAppPolicySetItem. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|itemType|String|policySetType of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|payloadId|String|PayloadId of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md)|
|settings|[mobileAppAssignmentSettings](../resources/intune-apps-mobileAppAssignmentSettings.md)|Settings of the MobileAppPolicySetItem.|
|status|Enumeration|Status of the PolicySetItem. Inherited from [policySetItem](../resources/policySetItem.md). Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
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
  "intent": "String",
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

