---
title: "managedDevice resource type"
description: "Devices that are managed or pre-enrolled through Intune"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# managedDevice resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Devices that are managed or pre-enrolled through Intune

## Methods

| Method                                                                                                        | Return Type                                         | Description                                                                           |
| :------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------- | :------------------------------------------------------------------------------------ |
| [List managedDevice](../api/intune-manageddevice-list.md)                                                     | [managedDevice](intune-managedDevice.md) collection | List properties and relationships of a managedDevice object.                          |
| [Create managedDevice](../api/intune-manageddevice-create.md)                                                 | [managedDevice](intune-managedDevice.md)            | Create a new managedDevice object.                                                    |
| [Get managedDevice](../api/intune-manageddevice-get.md)                                                       | [managedDevice](intune-managedDevice.md)            | Read properties and relationships of a managedDevice object.                          |
| [Update managedDevice](../api/intune-manageddevice-update.md)                                                 | [managedDevice](intune-managedDevice.md)            | Update the properties of a managedDevice object.                                      |
| [Delete managedDevice](../api/intune-manageddevice-delete.md)                                                 |                                                     | Delete a managedDevice object.                                                        |
| [bypassActivationLock](../api/intune-manageddevice-bypassActivationLock.md)                                   |                                                     | Bypass activation lock                                                                |
| [cleanWindowsDevice](../api/intune-manageddevice-cleanWindowsDevice.md)                                       |                                                     | Clean Windows device                                                                  |
| [createDeviceLogCollectionRequest](../api/intune-manageddevice-createDeviceLogCollectionRequest.md)           | deviceLogCollectionResponse                         |                                                                                       |
| [deleteUserFromSharedAppleDevice](../api/intune-manageddevice-deleteUserFromSharedAppleDevice.md)             |                                                     | Delete user from shared Apple device                                                  |
| [disableLostMode](../api/intune-manageddevice-disableLostMode.md)                                             |                                                     | Disable lost mode                                                                     |
| [enableLostMode](../api/intune-manageddevice-enableLostMode.md)                                               |                                                     | Enable lost mode                                                                      |
| [executeAction](../api/intune-manageddevice-executeAction.md)                                                 | bulkManagedDeviceActionResult                       |                                                                                       |
| [locateDevice](../api/intune-manageddevice-locateDevice.md)                                                   |                                                     | Locate a device                                                                       |
| [logoutSharedAppleDeviceActiveUser](../api/intune-manageddevice-logoutSharedAppleDeviceActiveUser.md)         |                                                     | Logout shared Apple device active user                                                |
| [playLostModeSound](../api/intune-manageddevice-playLostModeSound.md)                                         |                                                     | Remote lock                                                                           |
| [rebootNow](../api/intune-manageddevice-rebootNow.md)                                                         |                                                     | Reboot device                                                                         |
| [recoverPasscode](../api/intune-manageddevice-recoverPasscode.md)                                             |                                                     | Recover passcode                                                                      |
| [remoteLock](../api/intune-manageddevice-remoteLock.md)                                                       |                                                     | Remote lock                                                                           |
| [requestRemoteAssistance](../api/intune-manageddevice-requestRemoteAssistance.md)                             |                                                     | Request remote assistance                                                             |
| [resetPasscode](../api/intune-manageddevice-resetPasscode.md)                                                 |                                                     | Reset passcode                                                                        |
| [retire](../api/intune-manageddevice-retire.md)                                                               |                                                     | Retire a device                                                                       |
| [revokeAppleVppLicenses](../api/intune-manageddevice-revokeAppleVppLicenses.md)                               |                                                     | Revoke all Apple Vpp licenses for a device                                            |
| [rotateBitLockerKeys](../api/intune-manageddevice-rotateBitLockerKeys.md)                                     |                                                     | Rotate BitLockerKeys                                                                  |
| [rotateFileVaultKey](../api/intune-manageddevice-rotateFileVaultKey.md)                                       |                                                     |                                                                                       |
| [sendCustomNotificationToCompanyPortal](../api/intune-manageddevice-sendCustomNotificationToCompanyPortal.md) |                                                     |                                                                                       |
| [setDeviceName](../api/intune-manageddevice-setDeviceName.md)                                                 |                                                     | Set device name of the device.                                                        |
| [shutDown](../api/intune-manageddevice-shutDown.md)                                                           |                                                     | Shut down device                                                                      |
| [syncDevice](../api/intune-manageddevice-syncDevice.md)                                                       |                                                     |                                                                                       |
| [triggerConfigurationManagerAction](../api/intune-manageddevice-triggerConfigurationManagerAction.md)         |                                                     | Trigger action on ConfigurationManager client                                         |
| [updateWindowsDeviceAccount](../api/intune-manageddevice-updateWindowsDeviceAccount.md)                       |                                                     |                                                                                       |
| [windowsDefenderScan](../api/intune-manageddevice-windowsDefenderScan.md)                                     |                                                     |                                                                                       |
| [windowsDefenderUpdateSignatures](../api/intune-manageddevice-windowsDefenderUpdateSignatures.md)             |                                                     |                                                                                       |
| [wipe](../api/intune-manageddevice-wipe.md)                                                                   |                                                     | Wipe a device                                                                         |
| [getFileVaultKey](../api/intune-manageddevice-getFileVaultKey.md)                                             | String                                              |                                                                                       |
| [List detectedApps](../api/intune-manageddevice-list-detectedapps.md)                                         | detectedApp                                         | Get the detectedApp from a detectedApps navigation property.                          |
| [Add detectedApps](../api/intune-manageddevice-post-detectedapps.md)                                          | detectedApp                                         | Add detectedApps by posting to the detectedApps collection.                           |
| [Get detectedApps](../api/intune-manageddevice-get-detectedapps.md)                                           | detectedApp                                         | Read the properties and relationships of a detectedApp object.                        |
| [Update detectedApps](../api/intune-manageddevice-update-detectedapps.md)                                     | detectedApp                                         | Update the properties of a detectedApps object.                                       |
| [Remove detectedApps](../api/intune-manageddevice-delete-detectedapps.md)                                     |                                                     | Remove a detectedApp object.                                                          |
| [List deviceCategory](../api/intune-manageddevice-list-devicecategory.md)                                     | deviceCategory                                      | Get the deviceCategory from a deviceCategory navigation property.                     |
| [Create deviceCategory](../api/intune-manageddevice-post-devicecategory.md)                                   | deviceCategory                                      | Create a new deviceCategory object.                                                   |
| [Get deviceCategory](../api/intune-manageddevice-get-devicecategory.md)                                       | deviceCategory                                      | Read the properties and relationships of a deviceCategory object.                     |
| [Update deviceCategory](../api/intune-manageddevice-update-devicecategory.md)                                 | deviceCategory                                      | Update the properties of a deviceCategory object.                                     |
| [Delete deviceCategory](../api/intune-manageddevice-delete-devicecategory.md)                                 |                                                     | Delete a deviceCategory object.                                                       |
| [List logCollectionRequests](../api/intune-manageddevice-list-logcollectionrequests.md)                       | deviceLogCollectionResponse                         | Get the deviceLogCollectionResponse from a logCollectionRequests navigation property. |
| [Create logCollectionRequests](../api/intune-manageddevice-post-logcollectionrequests.md)                     | deviceLogCollectionResponse                         | Create a new logCollectionRequests object.                                            |
| [Get logCollectionRequests](../api/intune-manageddevice-get-logcollectionrequests.md)                         | deviceLogCollectionResponse                         | Read the properties and relationships of a deviceLogCollectionResponse object.        |
| [Update logCollectionRequests](../api/intune-manageddevice-update-logcollectionrequests.md)                   | deviceLogCollectionResponse                         | Update the properties of a logCollectionRequests object.                              |
| [Delete logCollectionRequests](../api/intune-manageddevice-delete-logcollectionrequests.md)                   |                                                     | Delete a deviceLogCollectionResponse object.                                          |
| [List users](../api/intune-manageddevice-list-users.md)                                                       | user                                                | Get the user from a users navigation property.                                        |
| [Create users](../api/intune-manageddevice-post-users.md)                                                     | user                                                | Create a new users object.                                                            |
| [Get users](../api/intune-manageddevice-get-users.md)                                                         | user                                                | Read the properties and relationships of a user object.                               |
| [Update users](../api/intune-manageddevice-update-users.md)                                                   | user                                                | Update the properties of a users object.                                              |
| [Delete users](../api/intune-manageddevice-delete-users.md)                                                   |                                                     | Delete a user object.                                                                 |
| [List windowsProtectionState](../api/intune-manageddevice-list-windowsprotectionstate.md)                     | windowsProtectionState                              | Get the windowsProtectionState from a windowsProtectionState navigation property.     |
| [Create windowsProtectionState](../api/intune-manageddevice-post-windowsprotectionstate.md)                   | windowsProtectionState                              | Create a new windowsProtectionState object.                                           |
| [Get windowsProtectionState](../api/intune-manageddevice-get-windowsprotectionstate.md)                       | windowsProtectionState                              | Read the properties and relationships of a windowsProtectionState object.             |
| [Update windowsProtectionState](../api/intune-manageddevice-update-windowsprotectionstate.md)                 | windowsProtectionState                              | Update the properties of a windowsProtectionState object.                             |
| [Delete windowsProtectionState](../api/intune-manageddevice-delete-windowsprotectionstate.md)                 |                                                     | Delete a windowsProtectionState object.                                               |

## Properties

| Property                                  | Type                                                                                                   | Description                                                                                                                                                                                              |
| :---------------------------------------- | :----------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| aadRegistered                             | Boolean                                                                                                | Whether the device is Azure Active Directory registered. This property is read-only.                                                                                                                     |
| activationLockBypassCode                  | String                                                                                                 | Code that allows the Activation Lock on a device to be bypassed. This property is read-only.                                                                                                             |
| androidSecurityPatchLevel                 | String                                                                                                 | Android security patch level. This property is read-only.                                                                                                                                                |
| autopilotEnrolled                         | Boolean                                                                                                | Reports if the managed device is enrolled via auto-pilot. This property is read-only.                                                                                                                    |
| azureADDeviceId                           | String                                                                                                 | The unique identifier for the Azure Active Directory device. Read only. This property is read-only.                                                                                                      |
| azureADRegistered                         | Boolean                                                                                                | Whether the device is Azure Active Directory registered. This property is read-only.                                                                                                                     |
| azureActiveDirectoryDeviceId              | String                                                                                                 | The unique identifier for the Azure Active Directory device. Read only. This property is read-only.                                                                                                      |
| chassisType                               | String                                                                                                 | Chassis type of the device. This property is read-only.                                                                                                                                                  |
| complianceGracePeriodExpirationDateTime   | DateTimeOffset                                                                                         | The DateTime when device compliance grace period expires. This property is read-only.                                                                                                                    |
| complianceState                           | String                                                                                                 | Compliance state of the device. This property is read-only.                                                                                                                                              |
| configurationManagerClientEnabledFeatures | [configurationManagerClientEnabledFeatures](../resources/configurationmanagerclientenabledfeatures.md) | ConfigrMgr client enabled features. This property is read-only.                                                                                                                                          |
| configurationManagerClientHealthState     | [configurationManagerClientHealthState](../resources/configurationmanagerclienthealthstate.md)         | Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent                                                                                                         |
| configurationManagerClientInformation     | [configurationManagerClientInformation](../resources/configurationmanagerclientinformation.md)         | Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent                                                                                 |
| deviceActionResults                       | [deviceActionResult](../resources/deviceactionresult.md) collection                                    | List of ComplexType deviceActionResult objects. This property is read-only.                                                                                                                              |
| deviceCategoryDisplayName                 | String                                                                                                 | Device category display name. This property is read-only.                                                                                                                                                |
| deviceEnrollmentType                      | String                                                                                                 | Enrollment type of the device. This property is read-only.                                                                                                                                               |
| deviceHealthAttestationState              | [deviceHealthAttestationState](../resources/devicehealthattestationstate.md)                           | The device health attestation state. This property is read-only.                                                                                                                                         |
| deviceName                                | String                                                                                                 | Name of the device. This property is read-only.                                                                                                                                                          |
| deviceRegistrationState                   | String                                                                                                 | Device registration state. This property is read-only.                                                                                                                                                   |
| deviceType                                | String                                                                                                 | Platform of the device. This property is read-only.                                                                                                                                                      |
| easActivated                              | Boolean                                                                                                | Whether the device is Exchange ActiveSync activated. This property is read-only.                                                                                                                         |
| easActivationDateTime                     | DateTimeOffset                                                                                         | Exchange ActivationSync activation time of the device. This property is read-only.                                                                                                                       |
| easDeviceId                               | String                                                                                                 | Exchange ActiveSync Id of the device. This property is read-only.                                                                                                                                        |
| emailAddress                              | String                                                                                                 | Email(s) for the user associated with the device. This property is read-only.                                                                                                                            |
| enrolledDateTime                          | DateTimeOffset                                                                                         | Enrollment time of the device. This property is read-only.                                                                                                                                               |
| ethernetMacAddress                        | String                                                                                                 | Ethernet MAC. This property is read-only.                                                                                                                                                                |
| exchangeAccessState                       | String                                                                                                 | The Access State of the device in Exchange. This property is read-only.                                                                                                                                  |
| exchangeAccessStateReason                 | String                                                                                                 | The reason for the device's access state in Exchange. This property is read-only.                                                                                                                        |
| exchangeLastSuccessfulSyncDateTime        | DateTimeOffset                                                                                         | Last time the device contacted Exchange. This property is read-only.                                                                                                                                     |
| freeStorageSpaceInBytes                   | Int64                                                                                                  | Free Storage in Bytes. This property is read-only.                                                                                                                                                       |
| hardwareInformation                       | [hardwareInformation](../resources/hardwareinformation.md)                                             | The hardward details for the device.  Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.                                                          |
| iccid                                     | String                                                                                                 | Integrated Circuit Card Identifier, it is A SIM card's unique identification number. This property is read-only.                                                                                         |
| id                                        | String                                                                                                 | Unique Identifier for the device. This property is read-only. Read-only.                                                                                                                                 |
| imei                                      | String                                                                                                 | IMEI. This property is read-only.                                                                                                                                                                        |
| isEncrypted                               | Boolean                                                                                                | Device encryption status. This property is read-only.                                                                                                                                                    |
| isSupervised                              | Boolean                                                                                                | Device supervised status. This property is read-only.                                                                                                                                                    |
| jailBroken                                | String                                                                                                 | whether the device is jail broken or rooted. This property is read-only.                                                                                                                                 |
| joinType                                  | String                                                                                                 | Device join type                                                                                                                                                                                         |
| lastSyncDateTime                          | DateTimeOffset                                                                                         | The date and time that the device last completed a successful sync with Intune. This property is read-only.                                                                                              |
| lostModeState                             | String                                                                                                 | Indicates if Lost mode is enabled or disabled. This property is read-only.                                                                                                                               |
| managedDeviceName                         | String                                                                                                 | Automatically generated name to identify a device. Can be overwritten to a user friendly name.                                                                                                           |
| managedDeviceOwnerType                    | String                                                                                                 | Ownership of the device. Can be 'company' or 'personal'                                                                                                                                                  |
| managementAgent                           | String                                                                                                 | Management channel of the device. Intune, EAS, etc. This property is read-only.                                                                                                                          |
| managementCertificateExpirationDate       | DateTimeOffset                                                                                         | Reports device management certificate expiration date. This property is read-only.                                                                                                                       |
| managementState                           | String                                                                                                 | Management state of the device. This property is read-only.                                                                                                                                              |
| manufacturer                              | String                                                                                                 | Manufacturer of the device. This property is read-only.                                                                                                                                                  |
| meid                                      | String                                                                                                 | MEID. This property is read-only.                                                                                                                                                                        |
| model                                     | String                                                                                                 | Model of the device. This property is read-only.                                                                                                                                                         |
| notes                                     | String                                                                                                 | Notes on the device created by IT Admin                                                                                                                                                                  |
| operatingSystem                           | String                                                                                                 | Operating system of the device. Windows, iOS, etc. This property is read-only.                                                                                                                           |
| osVersion                                 | String                                                                                                 | Operating system version of the device. This property is read-only.                                                                                                                                      |
| ownerType                                 | String                                                                                                 | Ownership of the device. Can be 'company' or 'personal'                                                                                                                                                  |
| partnerReportedThreatState                | String                                                                                                 | Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read Only. This property is read-only.                                                  |
| phoneNumber                               | String                                                                                                 | Phone number of the device. This property is read-only.                                                                                                                                                  |
| physicalMemoryInBytes                     | Int64                                                                                                  | Total Memory in Bytes. This property is read-only.                                                                                                                                                       |
| preferMdmOverGroupPolicyAppliedDateTime   | DateTimeOffset                                                                                         | Reports the DateTime the preferMdmOverGroupPolicy setting was set.  When set, the Intune MDM settings will override Group Policy settings if there is a conflict. Read Only. This property is read-only. |
| processorArchitecture                     | String                                                                                                 | Processor architecture. This property is read-only.                                                                                                                                                      |
| remoteAssistanceSessionErrorDetails       | String                                                                                                 | An error string that identifies issues when creating Remote Assistance session objects. This property is read-only.                                                                                      |
| remoteAssistanceSessionUrl                | String                                                                                                 | Url that allows a Remote Assistance session to be established with the device. This property is read-only.                                                                                               |
| requireUserEnrollmentApproval             | Boolean                                                                                                | Reports if the managed iOS device is user approval enrollment. This property is read-only.                                                                                                               |
| retireAfterDateTime                       | DateTimeOffset                                                                                         | Indicates the time after when a device will be auto retired because of scheduled action. This property is read-only.                                                                                     |
| roleScopeTagIds                           | String collection                                                                                      | List of Scope Tag IDs for this Device instance.                                                                                                                                                          |
| serialNumber                              | String                                                                                                 | SerialNumber. This property is read-only.                                                                                                                                                                |
| skuFamily                                 | String                                                                                                 | Device sku family                                                                                                                                                                                        |
| specificationVersion                      | String                                                                                                 | Specification version. This property is read-only.                                                                                                                                                       |
| subscriberCarrier                         | String                                                                                                 | Subscriber Carrier. This property is read-only.                                                                                                                                                          |
| totalStorageSpaceInBytes                  | Int64                                                                                                  | Total Storage in Bytes. This property is read-only.                                                                                                                                                      |
| udid                                      | String                                                                                                 | Unique Device Identifier for iOS and macOS devices. This property is read-only.                                                                                                                          |
| userDisplayName                           | String                                                                                                 | User display name. This property is read-only.                                                                                                                                                           |
| userId                                    | String                                                                                                 | Unique Identifier for the user associated with the device. This property is read-only.                                                                                                                   |
| userPrincipalName                         | String                                                                                                 | Device user principal name. This property is read-only.                                                                                                                                                  |
| usersLoggedOn                             | [loggedOnUser](../resources/loggedonuser.md) collection                                                | Indicates the last logged on users of a device. This property is read-only.                                                                                                                              |
| wiFiMacAddress                            | String                                                                                                 | Wi-Fi MAC. This property is read-only.                                                                                                                                                                   |
| windowsActiveMalwareCount                 | Int32                                                                                                  | Count of active malware for this windows device. This property is read-only.                                                                                                                             |
| windowsRemediatedMalwareCount             | Int32                                                                                                  | Count of remediated malware for this windows device. This property is read-only.                                                                                                                         |

## Relationships

| Relationship           | Type                                                                                  | Description                                           |
| :--------------------- | :------------------------------------------------------------------------------------ | :---------------------------------------------------- |
| detectedApps           | [detectedApp](../resources/detectedapp.md) collection                                 | All applications currently installed on the device    |
| deviceCategory         | [deviceCategory](../resources/devicecategory.md)                                      | Device category                                       |
| logCollectionRequests  | [deviceLogCollectionResponse](../resources/devicelogcollectionresponse.md) collection | List of log collection requests                       |
| users                  | [user](../resources/user.md) collection                                               | The primary users associated with the managed device. |
| windowsProtectionState | [windowsProtectionState](../resources/windowsprotectionstate.md)                      | The device protection status.                         |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "aadRegistered": "Boolean",
  "activationLockBypassCode": "String",
  "androidSecurityPatchLevel": "String",
  "autopilotEnrolled": "Boolean",
  "azureADDeviceId": "String",
  "azureADRegistered": "Boolean",
  "azureActiveDirectoryDeviceId": "String",
  "chassisType": "unknown | desktop | laptop | worksWorkstation | enterpriseServer | phone | tablet | mobileOther | mobileUnknown",
  "complianceGracePeriodExpirationDateTime": "DateTimeOffset",
  "complianceState": "unknown | compliant | noncompliant | conflict | error | inGracePeriod | configManager",
  "configurationManagerClientEnabledFeatures": {"@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"},
  "configurationManagerClientHealthState": {"@odata.type": "microsoft.graph.configurationManagerClientHealthState"},
  "configurationManagerClientInformation": {"@odata.type": "microsoft.graph.configurationManagerClientInformation"},
  "deviceActionResults": [{"@odata.type": "microsoft.graph.deviceActionResult"}],
  "deviceCategoryDisplayName": "String",
  "deviceEnrollmentType": "unknown | userEnrollment | deviceEnrollmentManager | appleBulkWithUser | appleBulkWithoutUser | windowsAzureADJoin | windowsBulkUserless | windowsAutoEnrollment | windowsBulkAzureDomainJoin | windowsCoManagement | appleUserEnrollment | appleUserEnrollmentWithServiceAccount | azureAdJoinUsingAzureVmExtension | androidEnterpriseDedicatedDevice | androidEnterpriseFullyManaged | androidEnterpriseCorporateWorkProfile",
  "deviceHealthAttestationState": {"@odata.type": "microsoft.graph.deviceHealthAttestationState"},
  "deviceName": "String",
  "deviceRegistrationState": "notRegistered | registered | revoked | keyConflict | approvalPending | certificateReset | notRegisteredPendingEnrollment | unknown",
  "deviceType": "desktop | windowsRT | winMO6 | nokia | windowsPhone | mac | winCE | winEmbedded | iPhone | iPad | iPod | android | iSocConsumer | unix | macMDM | holoLens | surfaceHub | androidForWork | androidEnterprise | windows10x | androidnGMS | blackberry | palm | unknown",
  "easActivated": "Boolean",
  "easActivationDateTime": "DateTimeOffset",
  "easDeviceId": "String",
  "emailAddress": "String",
  "enrolledDateTime": "DateTimeOffset",
  "ethernetMacAddress": "String",
  "exchangeAccessState": "none | unknown | allowed | blocked | quarantined",
  "exchangeAccessStateReason": "none | unknown | exchangeGlobalRule | exchangeIndividualRule | exchangeDeviceRule | exchangeUpgrade | exchangeMailboxPolicy | other | compliant | notCompliant | notEnrolled | unknownLocation | mfaRequired | azureADBlockDueToAccessPolicy | compromisedPassword | deviceNotKnownWithManagedApp",
  "exchangeLastSuccessfulSyncDateTime": "DateTimeOffset",
  "freeStorageSpaceInBytes": "Int64",
  "hardwareInformation": {"@odata.type": "microsoft.graph.hardwareInformation"},
  "iccid": "String",
  "id": "String (identifier)",
  "imei": "String",
  "isEncrypted": "Boolean",
  "isSupervised": "Boolean",
  "jailBroken": "String",
  "joinType": "unknown | azureADJoined | azureADRegistered | hybridAzureADJoined",
  "lastSyncDateTime": "DateTimeOffset",
  "lostModeState": "disabled | enabled",
  "managedDeviceName": "String",
  "managedDeviceOwnerType": "unknown | company | personal",
  "managementAgent": "eas | mdm | easMdm | intuneClient | easIntuneClient | configurationManagerClient | configurationManagerClientMdm | configurationManagerClientMdmEas | unknown | jamf | googleCloudDevicePolicyController | microsoft365ManagedMdm | windowsManagementCloudApi",
  "managementCertificateExpirationDate": "DateTimeOffset",
  "managementState": "managed | retirePending | retireFailed | wipePending | wipeFailed | unhealthy | deletePending | retireIssued | wipeIssued | wipeCanceled | retireCanceled | discovered",
  "manufacturer": "String",
  "meid": "String",
  "model": "String",
  "notes": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "ownerType": "unknown | company | personal",
  "partnerReportedThreatState": "unknown | activated | deactivated | secured | lowSeverity | mediumSeverity | highSeverity | unresponsive | compromised | misconfigured",
  "phoneNumber": "String",
  "physicalMemoryInBytes": "Int64",
  "preferMdmOverGroupPolicyAppliedDateTime": "DateTimeOffset",
  "processorArchitecture": "unknown | x86 | x64 | arm | arM64",
  "remoteAssistanceSessionErrorDetails": "String",
  "remoteAssistanceSessionUrl": "String",
  "requireUserEnrollmentApproval": "Boolean",
  "retireAfterDateTime": "DateTimeOffset",
  "roleScopeTagIds": ["String"],
  "serialNumber": "String",
  "skuFamily": "String",
  "specificationVersion": "String",
  "subscriberCarrier": "String",
  "totalStorageSpaceInBytes": "Int64",
  "udid": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "usersLoggedOn": [{"@odata.type": "microsoft.graph.loggedOnUser"}],
  "wiFiMacAddress": "String",
  "windowsActiveMalwareCount": "Int32",
  "windowsRemediatedMalwareCount": "Int32"
}
```