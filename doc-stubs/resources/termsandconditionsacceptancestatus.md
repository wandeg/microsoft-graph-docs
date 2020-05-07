---
title: "termsAndConditionsAcceptanceStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# termsAndConditionsAcceptanceStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List termsAndConditions](../api/termsandconditionsacceptancestatus-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditions from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/termsandconditionsacceptancestatus-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[Remove termsAndConditions](../api/termsandconditionsacceptancestatus-delete-termsandconditions.md)|None|Remove a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus from the acceptanceStatuses navigation property.|
|[Create acceptanceStatuses](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Create a new acceptanceStatuses object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptedDateTime|DateTimeOffset|**TODO: Add Description**|
|acceptedVersion|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": "Integer",
  "acceptedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

