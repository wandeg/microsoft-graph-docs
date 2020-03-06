---
title: "hardwareInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# hardwareInformation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|cellularTechnology|String|Cellular technology of the device|
|deviceFullQualifiedDomainName|String|Returns the fully qualified domain name of the device (if any). If the device is not domain-joined, it returns an empty string. |
|deviceGuardLocalSystemAuthorityCredentialGuardState|Enumeration|Local System Authority (LSA) credential guard status. . Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|Enumeration|Virtualization-based security hardware requirement status. Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|Enumeration|Virtualization-based security status. . Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|freeStorageSpace|Int64|Free storage space of the device.|
|imei|String|IMEI|
|isEncrypted|Boolean|Encryption status of the device|
|isSharedDevice|Boolean|Shared iPad|
|isSupervised|Boolean|Supervised mode of the device|
|manufacturer|String|Manufacturer of the device|
|meid|String|MEID|
|model|String|Model of the device|
|operatingSystemEdition|String|String that specifies the OS edition.|
|operatingSystemLanguage|String|Operating system language of the device|
|osBuildNumber|String|Operating System Build Number on Android device|
|phoneNumber|String|Phone number of the device|
|serialNumber|String|Serial number.|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/sharedappledeviceuser.md) collection|All users on the shared Apple device|
|subscriberCarrier|String|Subscriber carrier of the device|
|totalStorageSpace|Int64|Total storage space of the device.|
|tpmSpecificationVersion|String|String that specifies the specification version.|
|wifiMac|String|WiFi MAC address of the device|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String"
}
```

