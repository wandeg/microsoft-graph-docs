---
title: "enrollmentRestrictionsConfigurationPolicySetItem resource type"
description: "A class containing the properties used for enrollment restriction PolicySetItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enrollmentRestrictionsConfigurationPolicySetItem resource type


Namespace: microsoft.graph

A class containing the properties used for enrollment restriction PolicySetItem.


Inherits from [policySetItem](../resources/policysetitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List enrollmentRestrictionsConfigurationPolicySetItems](../api/enrollmentrestrictionsconfigurationpolicysetitem-list.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md) collection|List properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md) objects.|
|[Get enrollmentRestrictionsConfigurationPolicySetItem](../api/enrollmentrestrictionsconfigurationpolicysetitem-get.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md)|Read properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md) object.|
|[Create enrollmentRestrictionsConfigurationPolicySetItem](../api/enrollmentrestrictionsconfigurationpolicysetitem-create.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md)|Create a new [enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md) object.|
|[Delete enrollmentRestrictionsConfigurationPolicySetItem](../api/enrollmentrestrictionsconfigurationpolicysetitem-delete.md)|None|Deletes a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md).|
|[Update enrollmentRestrictionsConfigurationPolicySetItem](../api/enrollmentrestrictionsconfigurationpolicysetitem-update.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md)|Update the properties of a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/enrollmentrestrictionsconfigurationpolicysetitem.md) object.|

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
|limit|Int32|Limit of the EnrollmentRestrictionsConfigurationPolicySetItem.|
|payloadId|String|PayloadId of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md)|
|priority|Int32|Priority of the EnrollmentRestrictionsConfigurationPolicySetItem.|
|status|Enumeration|Status of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md). Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
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
  "priority": 1024,
  "limit": 1024
}
```

