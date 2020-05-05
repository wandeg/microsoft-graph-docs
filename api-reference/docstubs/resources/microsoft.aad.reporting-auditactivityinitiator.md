---
title: "auditActivityInitiator resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# auditActivityInitiator resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|app|[appIdentity](../resources/microsoft.aad.reporting-appidentity.md)|**TODO: Add Description**|
|user|[userIdentity](../resources/microsoft.aad.reporting-useridentity.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.auditActivityInitiator"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.auditActivityInitiator",
  "user": {
    "@odata.type": "Microsoft.AAD.Reporting.userIdentity"
  },
  "app": {
    "@odata.type": "Microsoft.AAD.Reporting.appIdentity"
  }
}
```

