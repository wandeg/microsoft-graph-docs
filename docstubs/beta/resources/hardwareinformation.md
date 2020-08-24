---
title: "hardwareInformation resource type"
description: "Hardware information of a given device."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# hardwareInformation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Hardware information of a given device.

## Properties

| Property                                                       | Type                                                                      | Description                                                                                                                                                  |
| :------------------------------------------------------------- | :------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| cellularTechnology                                             | String                                                                    | Cellular technology of the device                                                                                                                            |
| deviceFullQualifiedDomainName                                  | String                                                                    | Returns the fully qualified domain name of the device (if any). If the device is not domain-joined, it returns an empty string.                              |
| deviceGuardLocalSystemAuthorityCredentialGuardState            | String                                                                    | Local System Authority (LSA) credential guard status.                                                                                                        |
| deviceGuardVirtualizationBasedSecurityHardwareRequirementState | String                                                                    | Virtualization-based security hardware requirement status.                                                                                                   |
| deviceGuardVirtualizationBasedSecurityState                    | String                                                                    | Virtualization-based security status.                                                                                                                        |
| freeStorageSpace                                               | Int64                                                                     | Free storage space of the device.                                                                                                                            |
| imei                                                           | String                                                                    | IMEI                                                                                                                                                         |
| isEncrypted                                                    | Boolean                                                                   | Encryption status of the device                                                                                                                              |
| isSharedDevice                                                 | Boolean                                                                   | Shared iPad                                                                                                                                                  |
| isSupervised                                                   | Boolean                                                                   | Supervised mode of the device                                                                                                                                |
| manufacturer                                                   | String                                                                    | Manufacturer of the device                                                                                                                                   |
| meid                                                           | String                                                                    | MEID                                                                                                                                                         |
| model                                                          | String                                                                    | Model of the device                                                                                                                                          |
| operatingSystemEdition                                         | String                                                                    | String that specifies the OS edition.                                                                                                                        |
| operatingSystemLanguage                                        | String                                                                    | Operating system language of the device                                                                                                                      |
| operatingSystemProductType                                     | Int32                                                                     | Int that specifies the Windows Operating System ProductType. More details here https://go.microsoft.com/fwlink/?linkid=2126950. Valid values 0 to 2147483647 |
| osBuildNumber                                                  | String                                                                    | Operating System Build Number on Android device                                                                                                              |
| phoneNumber                                                    | String                                                                    | Phone number of the device                                                                                                                                   |
| serialNumber                                                   | String                                                                    | Serial number.                                                                                                                                               |
| sharedDeviceCachedUsers                                        | [sharedAppleDeviceUser](../resources/sharedappledeviceuser.md) collection | All users on the shared Apple device                                                                                                                         |
| subscriberCarrier                                              | String                                                                    | Subscriber carrier of the device                                                                                                                             |
| totalStorageSpace                                              | Int64                                                                     | Total storage space of the device.                                                                                                                           |
| tpmSpecificationVersion                                        | String                                                                    | String that specifies the specification version.                                                                                                             |
| wifiMac                                                        | String                                                                    | WiFi MAC address of the device                                                                                                                               |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "cellularTechnology": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "running | rebootRequired | notLicensed | notConfigured | virtualizationBasedSecurityNotRunning",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "meetHardwareRequirements | secureBootRequired | dmaProtectionRequired | hyperVNotSupportedForGuestVM | hyperVNotAvailable",
  "deviceGuardVirtualizationBasedSecurityState": "running | rebootRequired | require64BitArchitecture | notLicensed | notConfigured | doesNotMeetHardwareRequirements | other",
  "freeStorageSpace": "Int64",
  "imei": "String",
  "isEncrypted": "Boolean",
  "isSharedDevice": "Boolean",
  "isSupervised": "Boolean",
  "manufacturer": "String",
  "meid": "String",
  "model": "String",
  "operatingSystemEdition": "String",
  "operatingSystemLanguage": "String",
  "operatingSystemProductType": "Int32",
  "osBuildNumber": "String",
  "phoneNumber": "String",
  "serialNumber": "String",
  "sharedDeviceCachedUsers": [{"@odata.type": "microsoft.graph.sharedAppleDeviceUser"}],
  "subscriberCarrier": "String",
  "totalStorageSpace": "Int64",
  "tpmSpecificationVersion": "String",
  "wifiMac": "String"
}
```