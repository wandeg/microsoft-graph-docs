---
title: "deviceHealthAttestationState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthAttestationState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attestationIdentityKey|String|**TODO: Add Description**|
|bitLockerStatus|String|**TODO: Add Description**|
|bootAppSecurityVersion|String|**TODO: Add Description**|
|bootDebugging|String|**TODO: Add Description**|
|bootManagerSecurityVersion|String|**TODO: Add Description**|
|bootManagerVersion|String|**TODO: Add Description**|
|bootRevisionListInfo|String|**TODO: Add Description**|
|codeIntegrity|String|**TODO: Add Description**|
|codeIntegrityCheckVersion|String|**TODO: Add Description**|
|codeIntegrityPolicy|String|**TODO: Add Description**|
|contentNamespaceUrl|String|**TODO: Add Description**|
|contentVersion|String|**TODO: Add Description**|
|dataExcutionPolicy|String|**TODO: Add Description**|
|deviceHealthAttestationStatus|String|**TODO: Add Description**|
|earlyLaunchAntiMalwareDriverProtection|String|**TODO: Add Description**|
|healthAttestationSupportedStatus|String|**TODO: Add Description**|
|healthStatusMismatchInfo|String|**TODO: Add Description**|
|issuedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastUpdateDateTime|String|**TODO: Add Description**|
|operatingSystemKernelDebugging|String|**TODO: Add Description**|
|operatingSystemRevListInfo|String|**TODO: Add Description**|
|pcr0|String|**TODO: Add Description**|
|pcrHashAlgorithm|String|**TODO: Add Description**|
|resetCount|Int64|**TODO: Add Description**|
|restartCount|Int64|**TODO: Add Description**|
|safeMode|String|**TODO: Add Description**|
|secureBoot|String|**TODO: Add Description**|
|secureBootConfigurationPolicyFingerPrint|String|**TODO: Add Description**|
|testSigning|String|**TODO: Add Description**|
|tpmVersion|String|**TODO: Add Description**|
|virtualSecureMode|String|**TODO: Add Description**|
|windowsPE|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": "Integer",
  "restartCount": "Integer",
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```

