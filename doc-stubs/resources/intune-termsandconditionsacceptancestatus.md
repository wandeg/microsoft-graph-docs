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
|[List acceptanceStatuses](../api/intune-termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus from the acceptanceStatuses navigation property.|
|[Create acceptanceStatuses](../api/intune-termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md)|Create a new acceptanceStatuses object.|
|[Delete acceptanceStatuses](../api/intune-termsandconditions-delete-acceptancestatuses.md)|None|Delete a [termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) object.|
|[Update acceptanceStatuses](../api/intune-termsandconditions-update-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md)|Update the properties of an acceptanceStatuses object.|
|[Get acceptanceStatuses](../api/intune-termsandconditions-get-termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md)|Read the properties and relationships of a [termsAndConditionsAcceptanceStatus](../resources/intune-termsandconditionsacceptancestatus.md) object.|
|[List termsAndConditions](../api/intune-termsandconditionsacceptancestatus-list-termsandconditions.md)|[termsAndConditions](../resources/intune-termsandconditions.md) collection|Get the termsAndConditions from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/intune-termsandconditionsacceptancestatus-post-termsandconditions.md)|[termsAndConditions](../resources/intune-termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[Remove termsAndConditions](../api/intune-termsandconditionsacceptancestatus-delete-termsandconditions.md)|None|Remove a [termsAndConditions](../resources/intune-termsandconditions.md) object.|

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
|termsAndConditions|[termsAndConditions](../resources/intune-termsandconditions.md)|**TODO: Add Description**|

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

