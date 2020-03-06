---
title: "activityBasedTimeoutPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# activityBasedTimeoutPolicy resource type


Namespace: microsoft.graph




Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-get.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Read properties and relationships of the [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.|
|[Update activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-update.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Update the properties of a [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.|
|[List appliesTo](../api/activitybasedtimeoutpolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/activitybasedtimeoutpolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create appliesTo by posting to the appliesTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection| Inherited from [stsPolicy](../resources/stspolicy.md)|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection| Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activityBasedTimeoutPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

