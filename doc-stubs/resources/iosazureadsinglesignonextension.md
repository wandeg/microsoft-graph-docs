---
title: "iosAzureAdSingleSignOnExtension resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosAzureAdSingleSignOnExtension resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [iosSingleSignOnExtension](../resources/iossinglesignonextension.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurations|[keyTypedValuePair](../resources/keytypedvaluepair.md) collection|**TODO: Add Description**|
|enableSharedDeviceMode|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": "Boolean",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair"
    }
  ]
}
```

