---
title: "auditActivityInitiator resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# auditActivityInitiator resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|app|[appIdentity](../resources/microsoft.aad.reporting-appidentity.md)||
|user|[userIdentity](../resources/microsoft.aad.reporting-useridentity.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.auditActivityInitiator"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.auditActivityInitiator",
  "user": {
    "@odata.type": "Microsoft.AAD.Reporting.userIdentity",
    "id": "String",
    "displayName": "String",
    "ipAddress": "String",
    "userPrincipalName": "String"
  },
  "app": {
    "@odata.type": "Microsoft.AAD.Reporting.appIdentity",
    "appId": "String",
    "servicePrincipalId": "String",
    "servicePrincipalName": "String"
  }
}
```

