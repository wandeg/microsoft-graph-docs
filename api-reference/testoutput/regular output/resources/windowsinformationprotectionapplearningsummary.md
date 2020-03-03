---
title: "windowsInformationProtectionAppLearningSummary resource type"
description: "Windows Information Protection AppLearning Summary entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionAppLearningSummary resource type


Namespace: microsoft.graph

Windows Information Protection AppLearning Summary entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsInformationProtectionAppLearningSummaries](../api/windowsinformationprotectionapplearningsummary-list.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) collection|List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) objects.|
|[Get windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|
|[Create windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-create.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Create a new [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|
|[Delete windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-delete.md)|None|Deletes a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md).|
|[Update windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-update.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|
|[List windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-list-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) collection|Get the windowsInformationProtectionAppLearningSummaries from the windowsInformationProtectionAppLearningSummaries navigation property.|
|[Add windowsInformationProtectionAppLearningSummaries](../api/devicemanagement-post-windowsinformationprotectionapplearningsummaries.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Add windowsInformationProtectionAppLearningSummaries by posting to the windowsInformationProtectionAppLearningSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationName|String|Application Name|
|applicationType|Enumeration|Application Type. Possible values are: `universal`, `desktop`.|
|deviceCount|Int32|Device Count|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```

