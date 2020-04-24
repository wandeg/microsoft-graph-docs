---
title: "windowsEnrollmentStatusScreenSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsEnrollmentStatusScreenSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

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

