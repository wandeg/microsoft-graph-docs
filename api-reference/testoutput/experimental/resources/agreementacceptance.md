---
title: "agreementAcceptance resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# agreementAcceptance resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agreementAcceptance](../api/agreementacceptance-get.md)|[agreementAcceptance](../resources/agreementAcceptance.md)|Read properties and relationships of the [agreementAcceptance](../resources/agreementacceptance.md) object.|
|[Delete agreementAcceptance](../api/agreementacceptance-delete.md)|None|Deletes a [agreementAcceptance](../resources/agreementacceptance.md).|
|[Update agreementAcceptance](../api/agreementacceptance-update.md)|[agreementAcceptance](../resources/agreementAcceptance.md)|Update the properties of a [agreementAcceptance](../resources/agreementacceptance.md) object.|
|[List agreementAcceptances](../api/user-list-agreementacceptances.md)|[agreementAcceptance](../resources/agreementAcceptance.md) collection|Get the agreementAcceptances from the agreementAcceptances navigation property.|
|[Create agreementAcceptances](../api/user-post-agreementacceptances.md)|[agreementAcceptance](../resources/agreementAcceptance.md)|Create agreementAcceptances by posting to the agreementAcceptances collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|agreementFileId|String||
|agreementId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|recordedDateTime|DateTimeOffset||
|state|Enumeration|. Possible values are: `accepted`, `declined`.|
|userDisplayName|String||
|userEmail|String||
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
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

