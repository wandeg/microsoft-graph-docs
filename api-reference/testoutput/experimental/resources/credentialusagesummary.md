---
title: "credentialUsageSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# credentialUsageSummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List credentialUsageSummaries](../api/credentialusagesummary-list.md)|[credentialUsageSummary](../resources/credentialUsageSummary.md) collection|List properties and relationships of the [credentialUsageSummary](../resources/credentialusagesummary.md) objects.|
|[Get credentialUsageSummary](../api/credentialusagesummary-get.md)|[credentialUsageSummary](../resources/credentialUsageSummary.md)|Read properties and relationships of the [credentialUsageSummary](../resources/credentialusagesummary.md) object.|
|[Create credentialUsageSummary](../api/credentialusagesummary-create.md)|[credentialUsageSummary](../resources/credentialUsageSummary.md)|Create a new [credentialUsageSummary](../resources/credentialusagesummary.md) object.|
|[Delete credentialUsageSummary](../api/credentialusagesummary-delete.md)|None|Deletes a [credentialUsageSummary](../resources/credentialusagesummary.md).|
|[Update credentialUsageSummary](../api/credentialusagesummary-update.md)|[credentialUsageSummary](../resources/credentialUsageSummary.md)|Update the properties of a [credentialUsageSummary](../resources/credentialusagesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethod|Enumeration|. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|failureActivityCount|Int64||
|feature|Enumeration|. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|successfulActivityCount|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialUsageSummary",
  "id": "String (identifier)",
  "feature": "String",
  "successfulActivityCount": 1024,
  "failureActivityCount": 1024,
  "authMethod": "String"
}
```

