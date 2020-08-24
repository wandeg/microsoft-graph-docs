---
title: "comanagementEligibleDevice resource type"
description: "Device Co-Management eligibility state"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# comanagementEligibleDevice resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device Co-Management eligibility state

## Methods

| Method                                                                                  | Return Type                                                                   | Description                                                               |
| :-------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- | :------------------------------------------------------------------------ |
| [List comanagementEligibleDevice](../api/intune-comanagementeligibledevice-list.md)     | [comanagementEligibleDevice](intune-comanagementEligibleDevice.md) collection | List properties and relationships of a comanagementEligibleDevice object. |
| [Create comanagementEligibleDevice](../api/intune-comanagementeligibledevice-create.md) | [comanagementEligibleDevice](intune-comanagementEligibleDevice.md)            | Create a new comanagementEligibleDevice object.                           |
| [Get comanagementEligibleDevice](../api/intune-comanagementeligibledevice-get.md)       | [comanagementEligibleDevice](intune-comanagementEligibleDevice.md)            | Read properties and relationships of a comanagementEligibleDevice object. |
| [Update comanagementEligibleDevice](../api/intune-comanagementeligibledevice-update.md) | [comanagementEligibleDevice](intune-comanagementEligibleDevice.md)            | Update the properties of a comanagementEligibleDevice object.             |
| [Delete comanagementEligibleDevice](../api/intune-comanagementeligibledevice-delete.md) |                                                                               | Delete a comanagementEligibleDevice object.                               |

## Properties

| Property                 | Type   | Description                         |
| :----------------------- | :----- | :---------------------------------- |
| clientRegistrationStatus | String | ClientRegistrationStatus            |
| deviceName               | String | DeviceName                          |
| deviceType               | String | DeviceType                          |
| entitySource             | Int32  | EntitySource                        |
| id                       | String | Unique Id for the device Read-only. |
| managementAgents         | String | ManagementAgents                    |
| managementState          | String | ManagementState                     |
| manufacturer             | String | Manufacturer                        |
| mdmStatus                | String | MDMStatus                           |
| model                    | String | Model                               |
| osDescription            | String | OSDescription                       |
| osVersion                | String | OSVersion                           |
| ownerType                | String | OwnerType                           |
| referenceId              | String | ReferenceId                         |
| serialNumber             | String | SerialNumber                        |
| status                   | String | ComanagementEligibleStatus          |
| upn                      | String | UPN                                 |
| userEmail                | String | UserEmail                           |
| userId                   | String | UserId                              |
| userName                 | String | UserName                            |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDevice",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "clientRegistrationStatus": "notRegistered | registered | revoked | keyConflict | approvalPending | certificateReset | notRegisteredPendingEnrollment | unknown",
  "deviceName": "String",
  "deviceType": "desktop | windowsRT | winMO6 | nokia | windowsPhone | mac | winCE | winEmbedded | iPhone | iPad | iPod | android | iSocConsumer | unix | macMDM | holoLens | surfaceHub | androidForWork | androidEnterprise | windows10x | androidnGMS | blackberry | palm | unknown",
  "entitySource": "Int32",
  "id": "String (identifier)",
  "managementAgents": "eas | mdm | easMdm | intuneClient | easIntuneClient | configurationManagerClient | configurationManagerClientMdm | configurationManagerClientMdmEas | unknown | jamf | googleCloudDevicePolicyController | microsoft365ManagedMdm | windowsManagementCloudApi",
  "managementState": "managed | retirePending | retireFailed | wipePending | wipeFailed | unhealthy | deletePending | retireIssued | wipeIssued | wipeCanceled | retireCanceled | discovered",
  "manufacturer": "String",
  "mdmStatus": "String",
  "model": "String",
  "osDescription": "String",
  "osVersion": "String",
  "ownerType": "unknown | company | personal",
  "referenceId": "String",
  "serialNumber": "String",
  "status": "comanaged | eligible | eligibleButNotAzureAdJoined | needsOsUpdate | ineligible",
  "upn": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String"
}
```