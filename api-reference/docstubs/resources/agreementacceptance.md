---
title: "agreementAcceptance resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# agreementAcceptance resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List agreementAcceptances](../api/agreementacceptance-list.md)|[agreementAcceptance](../resources/agreementacceptance.md) collection|Get a list of the [agreementAcceptance](../resources/agreementacceptance.md) objects and their properties.|
|[Get agreementAcceptance](../api/agreementacceptance-get.md)|[agreementAcceptance](../resources/agreementacceptance.md)|Read the properties and relationships of an [agreementAcceptance](../resources/agreementacceptance.md) object.|
|[Create agreementAcceptance](../api/agreementacceptance-post-agreementacceptances.md)|[agreementAcceptance](../resources/agreementacceptance.md)|Create a new [agreementAcceptance](../resources/agreementacceptance.md) object.|
|[Delete agreementAcceptance](../api/agreementacceptance-delete.md)|None|Deletes an [agreementAcceptance](../resources/agreementacceptance.md) object.|
|[Update agreementAcceptance](../api/agreementacceptance-update.md)|[agreementAcceptance](../resources/agreementacceptance.md)|Update the properties of an [agreementAcceptance](../resources/agreementacceptance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|agreementFileId|String|**TODO: Add Description**|
|agreementId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|recordedDateTime|DateTimeOffset|**TODO: Add Description**|
|state|agreementAcceptanceState|**TODO: Add Description**. Possible values are: `accepted`, `declined`.|
|userDisplayName|String|**TODO: Add Description**|
|userEmail|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "id": "String (identifier)",
  "agreementId": "String",
  "userId": "String",
  "agreementFileId": "String",
  "recordedDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userEmail": "String",
  "state": "String"
}
```

