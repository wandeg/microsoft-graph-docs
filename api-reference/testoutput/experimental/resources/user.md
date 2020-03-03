---
title: "user resource type"
description: "Represents an Azure Active Directory user object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# user resource type

Represents an Azure Active Directory user object.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Delete user](../api/user-delete.md)|None|Deletes a [user](../resources/user.md).|
|[Update user](../api/user-update.md)|[user](../resources/user.md)|Update the properties of a [user](../resources/user.md) object.|
|[delta](../api/user-delta.md)|[user](../resources/user.md) collection||
|[checkMemberGroups](../api/user-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/user-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/user-getmembergroups.md)|String collection||
|[getMemberObjects](../api/user-getmemberobjects.md)|String collection||
|[restore](../api/user-restore.md)|[directoryObject](../resources/directoryObject.md)||
|[assignLicense](../api/user-assignlicense.md)|[user](../resources/user.md)||
|[changePassword](../api/user-changepassword.md)|None||
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)|Boolean||
|[revokeSignInSessions](../api/user-revokesigninsessions.md)|Boolean||
|[reprocessLicenseAssignment](../api/user-reprocesslicenseassignment.md)|[user](../resources/user.md)||
|[sendMail](../api/user-sendmail.md)|None||
|[getMailTips](../api/user-getmailtips.md)|[mailTips](../resources/mailTips.md) collection||
|[translateExchangeIds](../api/user-translateexchangeids.md)|[convertIdResult](../resources/convertIdResult.md) collection||
|[findMeetingTimes](../api/user-findmeetingtimes.md)|[meetingTimeSuggestionsResult](../resources/meetingTimeSuggestionsResult.md)||
|[exportDeviceAndAppManagementData](../api/user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/deviceAndAppManagementData.md)||
|[exportDeviceAndAppManagementData](../api/user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/deviceAndAppManagementData.md)||
|[getEffectiveDeviceEnrollmentConfigurations](../api/user-geteffectivedeviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md) collection||
|[removeAllDevicesFromManagement](../api/user-removealldevicesfrommanagement.md)|None||
|[getLoggedOnManagedDevices](../api/user-getloggedonmanageddevices.md)|[managedDevice](../resources/intune-devices-managedDevice.md) collection||
|[getManagedAppDiagnosticStatuses](../api/user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/managedAppDiagnosticStatus.md) collection||
|[getManagedAppPolicies](../api/user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/managedAppPolicy.md) collection||
|[wipeManagedAppRegistrationByDeviceTag](../api/user-wipemanagedappregistrationbydevicetag.md)|None||
|[wipeManagedAppRegistrationsByDeviceTag](../api/user-wipemanagedappregistrationsbydevicetag.md)|None||
|[getManagedDevicesWithAppFailures](../api/user-getmanageddeviceswithappfailures.md)|String collection||
|[exportPersonalData](../api/user-exportpersonaldata.md)|None||
|[Get userAnalytics](../api/useranalytics-get.md)|[userAnalytics](../resources/userAnalytics.md)|Read properties and relationships of the [userAnalytics](../resources/useranalytics.md) object.|
|[Get informationProtection](../api/informationprotection-get.md)|[informationProtection](../resources/informationProtection.md)|Read properties and relationships of the [informationProtection](../resources/informationprotection.md) object.|
|[List appRoleAssignments](../api/user-list-approleassignments.md)|[appRoleAssignment](../resources/appRoleAssignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Add appRoleAssignments](../api/user-post-approleassignments.md)|[appRoleAssignment](../resources/appRoleAssignment.md)|Add appRoleAssignments by posting to the appRoleAssignments collection.|
|[List createdObjects](../api/user-list-createdobjects.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the createdObjects navigation property.|
|[Create createdObjects](../api/user-post-createdobjects.md)|[directoryObject](../resources/directoryObject.md)|Create createdObjects by posting to the createdObjects collection.|
|[List directReports](../api/user-list-directreports.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the directReports navigation property.|
|[Create directReports](../api/user-post-directreports.md)|[directoryObject](../resources/directoryObject.md)|Create directReports by posting to the directReports collection.|
|[List licenseDetails](../api/user-list-licensedetails.md)|[licenseDetails](../resources/licenseDetails.md) collection|Get the licenseDetailses from the licenseDetails navigation property.|
|[Add licenseDetails](../api/user-post-licensedetails.md)|[licenseDetails](../resources/licenseDetails.md)|Add licenseDetails by posting to the licenseDetails collection.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryObject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[List memberOf](../api/user-list-memberof.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Create memberOf](../api/user-post-memberof.md)|[directoryObject](../resources/directoryObject.md)|Create memberOf by posting to the memberOf collection.|
|[List ownedDevices](../api/user-list-owneddevices.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the ownedDevices navigation property.|
|[Create ownedDevices](../api/user-post-owneddevices.md)|[directoryObject](../resources/directoryObject.md)|Create ownedDevices by posting to the ownedDevices collection.|
|[List ownedObjects](../api/user-list-ownedobjects.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the ownedObjects navigation property.|
|[Create ownedObjects](../api/user-post-ownedobjects.md)|[directoryObject](../resources/directoryObject.md)|Create ownedObjects by posting to the ownedObjects collection.|
|[List registeredDevices](../api/user-list-registereddevices.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the registeredDevices navigation property.|
|[Create registeredDevices](../api/user-post-registereddevices.md)|[directoryObject](../resources/directoryObject.md)|Create registeredDevices by posting to the registeredDevices collection.|
|[List scopedRoleMemberOf](../api/user-list-scopedrolememberof.md)|[scopedRoleMembership](../resources/scopedRoleMembership.md) collection|Get the scopedRoleMemberships from the scopedRoleMemberOf navigation property.|
|[Add scopedRoleMemberOf](../api/user-post-scopedrolememberof.md)|[scopedRoleMembership](../resources/scopedRoleMembership.md)|Add scopedRoleMemberOf by posting to the scopedRoleMemberOf collection.|
|[List transitiveMemberOf](../api/user-list-transitivememberof.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Create transitiveMemberOf](../api/user-post-transitivememberof.md)|[directoryObject](../resources/directoryObject.md)|Create transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Get outlookUser](../api/outlookuser-get.md)|[outlookUser](../resources/outlookUser.md)|Read properties and relationships of the [outlookUser](../resources/outlookuser.md) object.|
|[List messages](../api/user-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Add messages](../api/user-post-messages.md)|[message](../resources/message.md)|Add messages by posting to the messages collection.|
|[List joinedGroups](../api/user-list-joinedgroups.md)|[group](../resources/group.md) collection|Get the groups from the joinedGroups navigation property.|
|[Add joinedGroups](../api/user-post-joinedgroups.md)|[group](../resources/group.md)|Add joinedGroups by posting to the joinedGroups collection.|
|[List mailFolders](../api/user-list-mailfolders.md)|[mailFolder](../resources/mailFolder.md) collection|Get the mailFolders from the mailFolders navigation property.|
|[Add mailFolders](../api/user-post-mailfolders.md)|[mailFolder](../resources/mailFolder.md)|Add mailFolders by posting to the mailFolders collection.|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read properties and relationships of the [calendar](../resources/calendar.md) object.|
|[List calendars](../api/user-list-calendars.md)|[calendar](../resources/calendar.md) collection|Get the calendars from the calendars navigation property.|
|[Add calendars](../api/user-post-calendars.md)|[calendar](../resources/calendar.md)|Add calendars by posting to the calendars collection.|
|[List calendarGroups](../api/user-list-calendargroups.md)|[calendarGroup](../resources/calendarGroup.md) collection|Get the calendarGroups from the calendarGroups navigation property.|
|[Add calendarGroups](../api/user-post-calendargroups.md)|[calendarGroup](../resources/calendarGroup.md)|Add calendarGroups by posting to the calendarGroups collection.|
|[List calendarView](../api/user-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Add calendarView](../api/user-post-calendarview.md)|[event](../resources/event.md)|Add calendarView by posting to the calendarView collection.|
|[List events](../api/user-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Add events](../api/user-post-events.md)|[event](../resources/event.md)|Add events by posting to the events collection.|
|[List people](../api/user-list-people.md)|[person](../resources/person.md) collection|Get the persons from the people navigation property.|
|[Add people](../api/user-post-people.md)|[person](../resources/person.md)|Add people by posting to the people collection.|
|[List contacts](../api/user-list-contacts.md)|[contact](../resources/contact.md) collection|Get the contacts from the contacts navigation property.|
|[Add contacts](../api/user-post-contacts.md)|[contact](../resources/contact.md)|Add contacts by posting to the contacts collection.|
|[List contactFolders](../api/user-list-contactfolders.md)|[contactFolder](../resources/contactFolder.md) collection|Get the contactFolders from the contactFolders navigation property.|
|[Add contactFolders](../api/user-post-contactfolders.md)|[contactFolder](../resources/contactFolder.md)|Add contactFolders by posting to the contactFolders collection.|
|[Get inferenceClassification](../api/inferenceclassification-get.md)|[inferenceClassification](../resources/inferenceClassification.md)|Read properties and relationships of the [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilePhoto.md)|Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.|
|[List photos](../api/user-list-photos.md)|[profilePhoto](../resources/profilePhoto.md) collection|Get the profilePhotos from the photos navigation property.|
|[Add photos](../api/user-post-photos.md)|[profilePhoto](../resources/profilePhoto.md)|Add photos by posting to the photos collection.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of the [drive](../resources/drive.md) object.|
|[List drives](../api/user-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Add drives](../api/user-post-drives.md)|[drive](../resources/drive.md)|Add drives by posting to the drives collection.|
|[List followedSites](../api/user-list-followedsites.md)|[site](../resources/site.md) collection|Get the sites from the followedSites navigation property.|
|[Create followedSites](../api/user-post-followedsites.md)|[site](../resources/site.md)|Create followedSites by posting to the followedSites collection.|
|[List extensions](../api/user-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/user-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List agreementAcceptances](../api/user-list-agreementacceptances.md)|[agreementAcceptance](../resources/agreementAcceptance.md) collection|Get the agreementAcceptances from the agreementAcceptances navigation property.|
|[Create agreementAcceptances](../api/user-post-agreementacceptances.md)|[agreementAcceptance](../resources/agreementAcceptance.md)|Create agreementAcceptances by posting to the agreementAcceptances collection.|
|[List deviceEnrollmentConfigurations](../api/user-list-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md) collection|Get the deviceEnrollmentConfigurations from the deviceEnrollmentConfigurations navigation property.|
|[Add deviceEnrollmentConfigurations](../api/user-post-deviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md)|Add deviceEnrollmentConfigurations by posting to the deviceEnrollmentConfigurations collection.|
|[List managedDevices](../api/user-list-manageddevices.md)|[managedDevice](../resources/intune-devices-managedDevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Add managedDevices](../api/user-post-manageddevices.md)|[managedDevice](../resources/intune-devices-managedDevice.md)|Add managedDevices by posting to the managedDevices collection.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/managedAppRegistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Create managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/managedAppRegistration.md)|Create managedAppRegistrations by posting to the managedAppRegistrations collection.|
|[List windowsInformationProtectionDeviceRegistrations](../api/user-list-windowsinformationprotectiondeviceregistrations.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsInformationProtectionDeviceRegistration.md) collection|Get the windowsInformationProtectionDeviceRegistrations from the windowsInformationProtectionDeviceRegistrations navigation property.|
|[Create windowsInformationProtectionDeviceRegistrations](../api/user-post-windowsinformationprotectiondeviceregistrations.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsInformationProtectionDeviceRegistration.md)|Create windowsInformationProtectionDeviceRegistrations by posting to the windowsInformationProtectionDeviceRegistrations collection.|
|[List deviceManagementTroubleshootingEvents](../api/user-list-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md) collection|Get the deviceManagementTroubleshootingEvents from the deviceManagementTroubleshootingEvents navigation property.|
|[Add deviceManagementTroubleshootingEvents](../api/user-post-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md)|Add deviceManagementTroubleshootingEvents by posting to the deviceManagementTroubleshootingEvents collection.|
|[List mobileAppIntentAndStates](../api/user-list-mobileappintentandstates.md)|[mobileAppIntentAndState](../resources/mobileAppIntentAndState.md) collection|Get the mobileAppIntentAndStates from the mobileAppIntentAndStates navigation property.|
|[Add mobileAppIntentAndStates](../api/user-post-mobileappintentandstates.md)|[mobileAppIntentAndState](../resources/mobileAppIntentAndState.md)|Add mobileAppIntentAndStates by posting to the mobileAppIntentAndStates collection.|
|[List mobileAppTroubleshootingEvents](../api/user-list-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileAppTroubleshootingEvent.md) collection|Get the mobileAppTroubleshootingEvents from the mobileAppTroubleshootingEvents navigation property.|
|[Add mobileAppTroubleshootingEvents](../api/user-post-mobileapptroubleshootingevents.md)|[mobileAppTroubleshootingEvent](../resources/mobileAppTroubleshootingEvent.md)|Add mobileAppTroubleshootingEvents by posting to the mobileAppTroubleshootingEvents collection.|
|[List notifications](../api/user-list-notifications.md)|[notification](../resources/notification.md) collection|Get the notifications from the notifications navigation property.|
|[Add notifications](../api/user-post-notifications.md)|[notification](../resources/notification.md)|Add notifications by posting to the notifications collection.|
|[Get plannerUser](../api/planneruser-get.md)|[plannerUser](../resources/plannerUser.md)|Read properties and relationships of the [plannerUser](../resources/planneruser.md) object.|
|[Get officeGraphInsights](../api/officegraphinsights-get.md)|[officeGraphInsights](../resources/officeGraphInsights.md)|Read properties and relationships of the [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[Get userSettings](../api/usersettings-get.md)|[userSettings](../resources/userSettings.md)|Read properties and relationships of the [userSettings](../resources/usersettings.md) object.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of the [onenote](../resources/onenote.md) object.|
|[Get profile](../api/profile-get.md)|[profile](../resources/profile.md)|Read properties and relationships of the [profile](../resources/profile.md) object.|
|[List activities](../api/user-list-activities.md)|[userActivity](../resources/userActivity.md) collection|Get the userActivities from the activities navigation property.|
|[Add activities](../api/user-post-activities.md)|[userActivity](../resources/userActivity.md)|Add activities by posting to the activities collection.|
|[List devices](../api/user-list-devices.md)|[device](../resources/device.md) collection|Get the devices from the devices navigation property.|
|[Add devices](../api/user-post-devices.md)|[device](../resources/device.md)|Add devices by posting to the devices collection.|
|[List onlineMeetings](../api/user-list-onlinemeetings.md)|[onlineMeeting](../resources/onlineMeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Add onlineMeetings](../api/user-post-onlinemeetings.md)|[onlineMeeting](../resources/onlineMeeting.md)|Add onlineMeetings by posting to the onlineMeetings collection.|
|[Get presence](../api/presence-get.md)|[presence](../resources/presence.md)|Read properties and relationships of the [presence](../resources/presence.md) object.|
|[List chats](../api/user-list-chats.md)|[chat](../resources/chat.md) collection|Get the chats from the chats navigation property.|
|[Add chats](../api/user-post-chats.md)|[chat](../resources/chat.md)|Add chats by posting to the chats collection.|
|[List joinedTeams](../api/user-list-joinedteams.md)|[team](../resources/team.md) collection|Get the teams from the joinedTeams navigation property.|
|[Add joinedTeams](../api/user-post-joinedteams.md)|[team](../resources/team.md)|Add joinedTeams by posting to the joinedTeams collection.|
|[Get userTeamwork](../api/userteamwork-get.md)|[userTeamwork](../resources/userTeamwork.md)|Read properties and relationships of the [userTeamwork](../resources/userteamwork.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aboutMe|String||
|accountEnabled|Boolean||
|ageGroup|String||
|assignedLicenses|[assignedLicense](../resources/assignedLicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedPlan.md) collection||
|birthday|DateTimeOffset||
|businessPhones|String collection||
|city|String||
|companyName|String||
|consentProvidedForMinor|String||
|country|String||
|createdDateTime|DateTimeOffset||
|creationType|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|department|String||
|deviceEnrollmentLimit|Int32|The limit on the maximum number of devices that the user is permitted to enroll. Allowed values are 5 or 1000.|
|deviceKeys|[deviceKey](../resources/deviceKey.md) collection||
|displayName|String||
|employeeId|String||
|externalUserState|String||
|externalUserStateChangeDateTime|String||
|faxNumber|String||
|givenName|String||
|hireDate|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|identities|[objectIdentity](../resources/objectIdentity.md) collection||
|identityUserRisk|[identityUserRisk](../resources/identityUserRisk.md)||
|imAddresses|String collection||
|interests|String collection||
|isResourceAccount|Boolean||
|jobTitle|String||
|lastPasswordChangeDateTime|DateTimeOffset||
|legalAgeGroupClassification|String||
|licenseAssignmentStates|[licenseAssignmentState](../resources/licenseAssignmentState.md) collection||
|mail|String||
|mailboxSettings|[mailboxSettings](../resources/mailboxSettings.md)||
|mailNickname|String||
|mobilePhone|String||
|mySite|String||
|officeLocation|String||
|onPremisesDistinguishedName|String||
|onPremisesDomainName|String||
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](../resources/onPremisesExtensionAttributes.md)||
|onPremisesImmutableId|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onPremisesProvisioningError.md) collection||
|onPremisesSamAccountName|String||
|onPremisesSecurityIdentifier|String||
|onPremisesSyncEnabled|Boolean||
|onPremisesUserPrincipalName|String||
|otherMails|String collection||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordProfile.md)||
|pastProjects|String collection||
|postalCode|String||
|preferredDataLocation|String||
|preferredLanguage|String||
|preferredName|String||
|provisionedPlans|[provisionedPlan](../resources/provisionedPlan.md) collection||
|proxyAddresses|String collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|responsibilities|String collection||
|schools|String collection||
|showInAddressList|Boolean||
|signInActivity|[signInActivity](../resources/signInActivity.md)||
|signInSessionsValidFromDateTime|DateTimeOffset||
|skills|String collection||
|state|String||
|streetAddress|String||
|surname|String||
|usageLocation|String||
|userPrincipalName|String||
|userType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[userActivity](../resources/userActivity.md) collection||
|agreementAcceptances|[agreementAcceptance](../resources/agreementAcceptance.md) collection||
|analytics|[userAnalytics](../resources/userAnalytics.md)||
|appRoleAssignments|[appRoleAssignment](../resources/appRoleAssignment.md) collection||
|calendar|[calendar](../resources/calendar.md)||
|calendarGroups|[calendarGroup](../resources/calendarGroup.md) collection||
|calendars|[calendar](../resources/calendar.md) collection||
|calendarView|[event](../resources/event.md) collection||
|chats|[chat](../resources/chat.md) collection||
|contactFolders|[contactFolder](../resources/contactFolder.md) collection||
|contacts|[contact](../resources/contact.md) collection||
|createdObjects|[directoryObject](../resources/directoryObject.md) collection||
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/deviceEnrollmentConfiguration.md) collection|Get enrollment configurations targeted to the user|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md) collection|The list of troubleshooting events for this user.|
|devices|[device](../resources/device.md) collection||
|directReports|[directoryObject](../resources/directoryObject.md) collection||
|drive|[drive](../resources/drive.md)||
|drives|[drive](../resources/drive.md) collection||
|events|[event](../resources/event.md) collection||
|extensions|[extension](../resources/extension.md) collection||
|followedSites|[site](../resources/site.md) collection||
|inferenceClassification|[inferenceClassification](../resources/inferenceClassification.md)||
|informationProtection|[informationProtection](../resources/informationProtection.md)||
|insights|[officeGraphInsights](../resources/officeGraphInsights.md)||
|joinedGroups|[group](../resources/group.md) collection||
|joinedTeams|[team](../resources/team.md) collection||
|licenseDetails|[licenseDetails](../resources/licenseDetails.md) collection||
|mailFolders|[mailFolder](../resources/mailFolder.md) collection||
|managedAppRegistrations|[managedAppRegistration](../resources/managedAppRegistration.md) collection|Zero or more managed app registrations that belong to the user.|
|managedDevices|[managedDevice](../resources/intune-devices-managedDevice.md) collection|The managed devices associated with the user.|
|manager|[directoryObject](../resources/directoryObject.md)||
|memberOf|[directoryObject](../resources/directoryObject.md) collection||
|messages|[message](../resources/message.md) collection||
|mobileAppIntentAndStates|[mobileAppIntentAndState](../resources/mobileAppIntentAndState.md) collection|The list of troubleshooting events for this user.|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/mobileAppTroubleshootingEvent.md) collection|The list of mobile app troubleshooting events for this user.|
|notifications|[notification](../resources/notification.md) collection||
|onenote|[onenote](../resources/onenote.md)||
|onlineMeetings|[onlineMeeting](../resources/onlineMeeting.md) collection||
|outlook|[outlookUser](../resources/outlookUser.md)||
|ownedDevices|[directoryObject](../resources/directoryObject.md) collection||
|ownedObjects|[directoryObject](../resources/directoryObject.md) collection||
|people|[person](../resources/person.md) collection||
|photo|[profilePhoto](../resources/profilePhoto.md)||
|photos|[profilePhoto](../resources/profilePhoto.md) collection||
|planner|[plannerUser](../resources/plannerUser.md)||
|presence|[presence](../resources/presence.md)||
|profile|[profile](../resources/profile.md)||
|registeredDevices|[directoryObject](../resources/directoryObject.md) collection||
|scopedRoleMemberOf|[scopedRoleMembership](../resources/scopedRoleMembership.md) collection||
|settings|[userSettings](../resources/userSettings.md)||
|teamwork|[userTeamwork](../resources/userTeamwork.md)||
|transitiveMemberOf|[directoryObject](../resources/directoryObject.md) collection||
|windowsInformationProtectionDeviceRegistrations|[windowsInformationProtectionDeviceRegistration](../resources/windowsInformationProtectionDeviceRegistration.md) collection|Zero or more WIP device registrations that belong to the user.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity",
    "lastSignInDateTime": "String (timestamp)",
    "lastSignInRequestId": "String"
  },
  "accountEnabled": true,
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "Guid"
      ],
      "skuId": "Guid"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "String (timestamp)",
      "capabilityStatus": "String",
      "service": "String",
      "servicePlanId": "Guid"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "createdDateTime": "String (timestamp)",
  "creationType": "String",
  "department": "String",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey",
      "keyType": "String",
      "keyMaterial": "binary",
      "deviceId": "Guid"
    }
  ],
  "displayName": "String",
  "employeeId": "String",
  "faxNumber": "String",
  "givenName": "String",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity",
      "signInType": "String",
      "issuer": "String",
      "issuerAssignedId": "String"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "isResourceAccount": true,
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState",
      "assignedByGroup": "String",
      "state": "String",
      "error": "String"
    }
  ],
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes",
    "extensionAttribute1": "String",
    "extensionAttribute2": "String",
    "extensionAttribute3": "String",
    "extensionAttribute4": "String",
    "extensionAttribute5": "String",
    "extensionAttribute6": "String",
    "extensionAttribute7": "String",
    "extensionAttribute8": "String",
    "extensionAttribute9": "String",
    "extensionAttribute10": "String",
    "extensionAttribute11": "String",
    "extensionAttribute12": "String",
    "extensionAttribute13": "String",
    "extensionAttribute14": "String",
    "extensionAttribute15": "String"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "String",
      "category": "String",
      "propertyCausingError": "String",
      "occurredDateTime": "String (timestamp)"
    }
  ],
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
  "onPremisesDomainName": "String",
  "onPremisesSamAccountName": "String",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile",
    "password": "String",
    "forceChangePasswordNextSignIn": true,
    "forceChangePasswordNextSignInWithMfa": true
  },
  "officeLocation": "String",
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "String"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "externalUserState": "String",
  "externalUserStateChangeDateTime": "String",
  "userType": "String",
  "mailboxSettings": {
    "@odata.type": "microsoft.graph.mailboxSettings",
    "automaticRepliesSetting": {
      "@odata.type": "microsoft.graph.automaticRepliesSetting",
      "status": "String",
      "externalAudience": "String",
      "scheduledStartDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone",
        "dateTime": "String",
        "timeZone": "String"
      },
      "scheduledEndDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "internalReplyMessage": "String",
      "externalReplyMessage": "String"
    },
    "archiveFolder": "String",
    "language": {
      "@odata.type": "microsoft.graph.localeInfo",
      "locale": "String"
    },
    "delegateMeetingMessageDeliveryOptions": "String",
    "workingHours": {
      "@odata.type": "microsoft.graph.workingHours",
      "daysOfWeek": [
        "String"
      ],
      "startTime": "String (time of day)",
      "endTime": "String (time of day)",
      "timeZone": {
        "@odata.type": "microsoft.graph.timeZoneBase",
        "name": "String"
      }
    },
    "dateFormat": "String",
    "timeFormat": "String"
  },
  "identityUserRisk": {
    "@odata.type": "microsoft.graph.identityUserRisk",
    "level": "String",
    "lastChangedDateTime": "String (timestamp)"
  },
  "deviceEnrollmentLimit": 1024,
  "aboutMe": "String",
  "birthday": "String (timestamp)",
  "hireDate": "String (timestamp)",
  "interests": [
    "String"
  ],
  "mySite": "String",
  "pastProjects": [
    "String"
  ],
  "preferredName": "String",
  "responsibilities": [
    "String"
  ],
  "schools": [
    "String"
  ],
  "skills": [
    "String"
  ]
}
```

