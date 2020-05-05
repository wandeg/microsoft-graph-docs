---
title: "trustFramework resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# trustFramework resource type


Namespace: microsoft.cpim.api.dataModels

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trustFramework](../api/microsoft.cpim.api.datamodels-trustframework-get.md)|[trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md)|Read properties and relationships of a [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object.|
|[Update trustFramework](../api/microsoft.cpim.api.datamodels-trustframework-update.md)|[trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md)|Update the properties of a [trustFramework](../resources/microsoft.cpim.api.datamodels-trustframework.md) object.|
|[List policies](../api/microsoft.cpim.api.datamodels-trustframework-list-policies.md)|[trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md) collection|Get the trustFrameworkPolicies from the policies navigation property.|
|[Create policies](../api/microsoft.cpim.api.datamodels-trustframework-post-policies.md)|[trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md)|Create a new policies object.|
|[Delete policies](../api/microsoft.cpim.api.datamodels-trustframework-delete-policies.md)|None|Delete a policies object.|
|[Update policies](../api/microsoft.cpim.api.datamodels-trustframework-update-policies.md)|[trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md)|Update the properties of a policies object.|
|[Get trustFrameworkPolicy](../api/microsoft.cpim.api.datamodels-trustframeworkpolicy-get.md)|[trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md)|Read properties and relationships of a [trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md) object.|
|[List keySets](../api/microsoft.cpim.api.datamodels-trustframework-list-keysets.md)|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) collection|Get the trustFrameworkKeySets from the keySets navigation property.|
|[Create keySets](../api/microsoft.cpim.api.datamodels-trustframework-post-keysets.md)|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md)|Create a new keySets object.|
|[Delete keySets](../api/microsoft.cpim.api.datamodels-trustframework-delete-keysets.md)|None|Delete a keySets object.|
|[Update keySets](../api/microsoft.cpim.api.datamodels-trustframework-update-keysets.md)|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md)|Update the properties of a keySets object.|
|[Get trustFrameworkKeySet](../api/microsoft.cpim.api.datamodels-trustframeworkkeyset-get.md)|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md)|Read properties and relationships of a [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|keySets|[trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) collection|**TODO: Add Description**|
|policies|[trustFrameworkPolicy](../resources/microsoft.cpim.api.datamodels-trustframeworkpolicy.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.cpim.api.dataModels.trustFramework",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFramework",
  "id": "String (identifier)"
}
```

