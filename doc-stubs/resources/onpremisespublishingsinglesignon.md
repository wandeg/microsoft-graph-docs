---
title: "onPremisesPublishingSingleSignOn resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onPremisesPublishingSingleSignOn resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|KerberosSignOnSettings|[kerberosSignOnSettings](../resources/kerberossignonsettings.md)|**TODO: Add Description**|
|SingleSignOnMode|singleSignOnMode|**TODO: Add Description**. Possible values are: `none`, `onPremisesKerberos`, `saml`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesPublishingSingleSignOn",
  "SingleSignOnMode": "String",
  "KerberosSignOnSettings": {
    "@odata.type": "microsoft.graph.kerberosSignOnSettings"
  }
}
```

