---
title: "deviceHealthAttestationState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthAttestationState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attestationIdentityKey|String||
|bitLockerStatus|String||
|bootAppSecurityVersion|String||
|bootDebugging|String||
|bootManagerSecurityVersion|String||
|bootManagerVersion|String||
|bootRevisionListInfo|String||
|codeIntegrity|String||
|codeIntegrityCheckVersion|String||
|codeIntegrityPolicy|String||
|contentNamespaceUrl|String||
|contentVersion|String||
|dataExcutionPolicy|String||
|deviceHealthAttestationStatus|String||
|earlyLaunchAntiMalwareDriverProtection|String||
|healthAttestationSupportedStatus|String||
|healthStatusMismatchInfo|String||
|issuedDateTime|DateTimeOffset||
|lastUpdateDateTime|String||
|operatingSystemKernelDebugging|String||
|operatingSystemRevListInfo|String||
|pcr0|String||
|pcrHashAlgorithm|String||
|resetCount|Int64||
|restartCount|Int64||
|safeMode|String||
|secureBoot|String||
|secureBootConfigurationPolicyFingerPrint|String||
|testSigning|String||
|tpmVersion|String||
|virtualSecureMode|String||
|windowsPE|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "resetCount": 1024,
  "restartCount": 1024,
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

