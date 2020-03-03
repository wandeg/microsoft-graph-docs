---
title: "windowsEnrollmentStatusScreenSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsEnrollmentStatusScreenSettings resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|Allow or block user to use device before profile and app installation complete|
|allowDeviceUseOnInstallFailure|Boolean|Allow the user to continue using the device on installation failure|
|allowLogCollectionOnInstallFailure|Boolean|Allow or block log collection on installation failure|
|blockDeviceSetupRetryByUser|Boolean|Allow the user to retry the setup on installation failure|
|customErrorMessage|String|Set custom error message to show upon installation failure|
|hideInstallationProgress|Boolean|Show or hide installation progress to user|
|installProgressTimeoutInMinutes|Int32|Set installation progress timeout in minutes|

## Relationships
None

## JSON Representation
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

