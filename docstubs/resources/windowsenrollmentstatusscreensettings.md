---
title: "windowsEnrollmentStatusScreenSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsEnrollmentStatusScreenSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean||
|allowDeviceUseOnInstallFailure|Boolean||
|allowLogCollectionOnInstallFailure|Boolean||
|blockDeviceSetupRetryByUser|Boolean||
|customErrorMessage|String||
|hideInstallationProgress|Boolean||
|installProgressTimeoutInMinutes|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```

