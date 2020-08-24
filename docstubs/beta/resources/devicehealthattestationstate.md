﻿---
title: "deviceHealthAttestationState resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthAttestationState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property                                 | Type           | Description                                                                                                                           |
| :--------------------------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------ |
| attestationIdentityKey                   | String         | TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate. |
| bitLockerStatus                          | String         | On or Off of BitLocker Drive Encryption                                                                                               |
| bootAppSecurityVersion                   | String         | The security version number of the Boot Application                                                                                   |
| bootDebugging                            | String         | When bootDebugging is enabled, the device is used in development and testing                                                          |
| bootManagerSecurityVersion               | String         | The security version number of the Boot Application                                                                                   |
| bootManagerVersion                       | String         | The version of the Boot Manager                                                                                                       |
| bootRevisionListInfo                     | String         | The Boot Revision List that was loaded during initial boot on the attested device                                                     |
| codeIntegrity                            | String         | When code integrity is enabled, code execution is restricted to integrity verified code                                               |
| codeIntegrityCheckVersion                | String         | The version of the Boot Manager                                                                                                       |
| codeIntegrityPolicy                      | String         | The Code Integrity policy that is controlling the security of the boot environment                                                    |
| contentNamespaceUrl                      | String         | The DHA report version. (Namespace version)                                                                                           |
| contentVersion                           | String         | The HealthAttestation state schema version                                                                                            |
| dataExcutionPolicy                       | String         | DEP Policy defines a set of hardware and software technologies that perform additional checks on memory                               |
| deviceHealthAttestationStatus            | String         | The DHA report version. (Namespace version)                                                                                           |
| earlyLaunchAntiMalwareDriverProtection   | String         | ELAM provides protection for the computers in your network when they start up                                                         |
| healthAttestationSupportedStatus         | String         | This attribute indicates if DHA is supported for the device                                                                           |
| healthStatusMismatchInfo                 | String         | This attribute appears if DHA-Service detects an integrity issue                                                                      |
| issuedDateTime                           | DateTimeOffset | The DateTime when device was evaluated or issued to MDM                                                                               |
| lastUpdateDateTime                       | String         | The Timestamp of the last update.                                                                                                     |
| operatingSystemKernelDebugging           | String         | When operatingSystemKernelDebugging is enabled, the device is used in development and testing                                         |
| operatingSystemRevListInfo               | String         | The Operating System Revision List that was loaded during initial boot on the attested device                                         |
| pcr0                                     | String         | The measurement that is captured in PCR[0]                                                                                            |
| pcrHashAlgorithm                         | String         | Informational attribute that identifies the HASH algorithm that was used by TPM                                                       |
| resetCount                               | Int64          | The number of times a PC device has hibernated or resumed                                                                             |
| restartCount                             | Int64          | The number of times a PC device has rebooted                                                                                          |
| safeMode                                 | String         | Safe mode is a troubleshooting option for Windows that starts your computer in a limited state                                        |
| secureBoot                               | String         | When Secure Boot is enabled, the core components must have the correct cryptographic signatures                                       |
| secureBootConfigurationPolicyFingerPrint | String         | Fingerprint of the Custom Secure Boot Configuration Policy                                                                            |
| testSigning                              | String         | When test signing is allowed, the device does not enforce signature validation during boot                                            |
| tpmVersion                               | String         | The security version number of the Boot Application                                                                                   |
| virtualSecureMode                        | String         | VSM is a container that protects high value assets from a compromised kernel                                                          |
| windowsPE                                | String         | Operating system running with limited services that is used to prepare a computer for Windows                                         |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "attestationIdentityKey": "String",
  "bitLockerStatus": "String",
  "bootAppSecurityVersion": "String",
  "bootDebugging": "String",
  "bootManagerSecurityVersion": "String",
  "bootManagerVersion": "String",
  "bootRevisionListInfo": "String",
  "codeIntegrity": "String",
  "codeIntegrityCheckVersion": "String",
  "codeIntegrityPolicy": "String",
  "contentNamespaceUrl": "String",
  "contentVersion": "String",
  "dataExcutionPolicy": "String",
  "deviceHealthAttestationStatus": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "healthAttestationSupportedStatus": "String",
  "healthStatusMismatchInfo": "String",
  "issuedDateTime": "DateTimeOffset",
  "lastUpdateDateTime": "String",
  "operatingSystemKernelDebugging": "String",
  "operatingSystemRevListInfo": "String",
  "pcr0": "String",
  "pcrHashAlgorithm": "String",
  "resetCount": "Int64",
  "restartCount": "Int64",
  "safeMode": "String",
  "secureBoot": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "testSigning": "String",
  "tpmVersion": "String",
  "virtualSecureMode": "String",
  "windowsPE": "String"
}
```