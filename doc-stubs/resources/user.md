---
title: "user resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# user resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List invitedUser](../api/invitation-list-inviteduser.md)|[user](../resources/user.md) collection|Get the users from the invitedUser navigation property.|
|[Add invitedUser](../api/invitation-post-inviteduser.md)|[user](../resources/user.md)|Add invitedUser by posting to the invitedUser collection.|
|[Remove invitedUser](../api/invitation-delete-inviteduser.md)|None|Remove a [user](../resources/user.md) object.|
|[List users](../api/user-list.md)|[user](../resources/user.md) collection|Get a list of the [user](../resources/user.md) objects and their properties.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read the properties and relationships of a [user](../resources/user.md) object.|
|[Create user](../api/user-post-users.md)|[user](../resources/user.md)|Create a new [user](../resources/user.md) object.|
|[Delete user](../api/user-delete.md)|None|Deletes a [user](../resources/user.md) object.|
|[Update user](../api/user-update.md)|[user](../resources/user.md)|Update the properties of a [user](../resources/user.md) object.|
|[delta](../api/user-delta.md)|[user](../resources/user.md) collection|**TODO: Add Description**|
|[getEnabledUsersForLinkedIn](../api/user-getenabledusersforlinkedin.md)|[user](../resources/user.md) collection|**TODO: Add Description**|
|[getEnabledUsersForLinkedIn](../api/user-getenabledusersforlinkedin.md)|[user](../resources/user.md) collection|**TODO: Add Description**|
|[revokeLocalGrantByMid](../api/user-revokelocalgrantbymid.md)|String|**TODO: Add Description**|
|[notifyConsent](../api/user-notifyconsent.md)|None|**TODO: Add Description**|
|[checkMemberGroups](../api/user-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/user-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/user-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/user-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/user-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[assignLicense](../api/user-assignlicense.md)|[user](../resources/user.md)|**TODO: Add Description**|
|[changePassword](../api/user-changepassword.md)|None|**TODO: Add Description**|
|[revokeSignInSessions](../api/user-revokesigninsessions.md)|Boolean|**TODO: Add Description**|
|[reprocessLicenseAssignment](../api/user-reprocesslicenseassignment.md)|[user](../resources/user.md)|**TODO: Add Description**|
|[findMeetingTimes](../api/user-findmeetingtimes.md)|[meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md)|**TODO: Add Description**|
|[sendMail](../api/user-sendmail.md)|None|**TODO: Add Description**|
|[reminderView](../api/user-reminderview.md)|[reminder](../resources/reminder.md) collection|**TODO: Add Description**|
|[getMailTips](../api/user-getmailtips.md)|[mailTips](../resources/mailtips.md) collection|**TODO: Add Description**|
|[translateExchangeIds](../api/user-translateexchangeids.md)|[convertIdResult](../resources/convertidresult.md) collection|**TODO: Add Description**|
|[getIdentityProviderAccessToken](../api/user-getidentityprovideraccesstoken.md)|String|**TODO: Add Description**|
|[removeAllDevicesFromManagement](../api/user-removealldevicesfrommanagement.md)|None|**TODO: Add Description**|
|[getManagedAppDiagnosticStatuses](../api/user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-managedappdiagnosticstatus.md) collection|**TODO: Add Description**|
|[getManagedAppPolicies](../api/user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|**TODO: Add Description**|
|[wipeManagedAppRegistrationsByDeviceTag](../api/user-wipemanagedappregistrationsbydevicetag.md)|None|**TODO: Add Description**|
|[getLinkedInStatus](../api/user-getlinkedinstatus.md)|[linkedInStatus](../resources/linkedinstatus.md)|**TODO: Add Description**|
|[setLinkedInEnabled](../api/user-setlinkedinenabled.md)|None|**TODO: Add Description**|
|[setLinkedInStatus](../api/user-setlinkedinstatus.md)|None|**TODO: Add Description**|
|[revokeDualGrant](../api/user-revokedualgrant.md)|None|**TODO: Add Description**|
|[revokeLocalGrant](../api/user-revokelocalgrant.md)|String|**TODO: Add Description**|
|[exportPersonalData](../api/user-exportpersonaldata.md)|None|**TODO: Add Description**|
|[List appRoleAssignments](../api/user-list-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Create appRoleAssignments](../api/user-post-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Create a new appRoleAssignments object.|
|[Delete appRoleAssignments](../api/user-delete-approleassignments.md)|None|Delete an [appRoleAssignment](../resources/approleassignment.md) object.|
|[Update appRoleAssignments](../api/user-update-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Update the properties of an appRoleAssignments object.|
|[Get appRoleAssignments](../api/user-get-approleassignment.md)|[appRoleAssignment](../resources/approleassignment.md)|Read the properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.|
|[List ownedDevices](../api/user-list-owneddevices.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the ownedDevices navigation property.|
|[Add ownedDevices](../api/user-post-owneddevices.md)|[directoryObject](../resources/directoryobject.md)|Add ownedDevices by posting to the ownedDevices collection.|
|[Remove ownedDevices](../api/user-delete-owneddevices.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List registeredDevices](../api/user-list-registereddevices.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the registeredDevices navigation property.|
|[Add registeredDevices](../api/user-post-registereddevices.md)|[directoryObject](../resources/directoryobject.md)|Add registeredDevices by posting to the registeredDevices collection.|
|[Remove registeredDevices](../api/user-delete-registereddevices.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List manager](../api/user-list-manager.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the manager navigation property.|
|[Add manager](../api/user-post-manager.md)|[directoryObject](../resources/directoryobject.md)|Add manager by posting to the manager collection.|
|[Remove manager](../api/user-delete-manager.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List directReports](../api/user-list-directreports.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the directReports navigation property.|
|[Add directReports](../api/user-post-directreports.md)|[directoryObject](../resources/directoryobject.md)|Add directReports by posting to the directReports collection.|
|[Remove directReports](../api/user-delete-directreports.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List memberOf](../api/user-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/user-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/user-delete-memberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List createdObjects](../api/user-list-createdobjects.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdObjects navigation property.|
|[Add createdObjects](../api/user-post-createdobjects.md)|[directoryObject](../resources/directoryobject.md)|Add createdObjects by posting to the createdObjects collection.|
|[Remove createdObjects](../api/user-delete-createdobjects.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List oauth2PermissionGrants](../api/user-list-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|Get the oAuth2PermissionGrant from the oauth2PermissionGrants navigation property.|
|[Add oauth2PermissionGrants](../api/user-post-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Add oauth2PermissionGrants by posting to the oauth2PermissionGrants collection.|
|[Remove oauth2PermissionGrants](../api/user-delete-oauth2permissiongrants.md)|None|Remove an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.|
|[List ownedObjects](../api/user-list-ownedobjects.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the ownedObjects navigation property.|
|[Add ownedObjects](../api/user-post-ownedobjects.md)|[directoryObject](../resources/directoryobject.md)|Add ownedObjects by posting to the ownedObjects collection.|
|[Remove ownedObjects](../api/user-delete-ownedobjects.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List licenseDetails](../api/user-list-licensedetails.md)|[licenseDetails](../resources/licensedetails.md) collection|Get the licenseDetails from the licenseDetails navigation property.|
|[Create licenseDetails](../api/user-post-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Create a new licenseDetails object.|
|[Delete licenseDetails](../api/user-delete-licensedetails.md)|None|Delete a [licenseDetails](../resources/licensedetails.md) object.|
|[Update licenseDetails](../api/user-update-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Update the properties of a licenseDetails object.|
|[Get licenseDetails](../api/user-get-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Read the properties and relationships of a [licenseDetails](../resources/licensedetails.md) object.|
|[List transitiveMemberOf](../api/user-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/user-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/user-delete-transitivememberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List outlook](../api/user-list-outlook.md)|[outlookUser](../resources/outlookuser.md) collection|Get the outlookUsers from the outlook navigation property.|
|[Create outlook](../api/user-post-outlook.md)|[outlookUser](../resources/outlookuser.md)|Create a new outlook object.|
|[Delete outlook](../api/user-delete-outlook.md)|None|Delete an [outlookUser](../resources/outlookuser.md) object.|
|[Update outlook](../api/user-update-outlook.md)|[outlookUser](../resources/outlookuser.md)|Update the properties of an outlook object.|
|[Get outlook](../api/user-get-outlookuser.md)|[outlookUser](../resources/outlookuser.md)|Read the properties and relationships of an [outlookUser](../resources/outlookuser.md) object.|
|[List messages](../api/user-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Create messages](../api/user-post-messages.md)|[message](../resources/message.md)|Create a new messages object.|
|[Delete messages](../api/user-delete-messages.md)|None|Delete a [message](../resources/message.md) object.|
|[Update messages](../api/user-update-messages.md)|[message](../resources/message.md)|Update the properties of a messages object.|
|[Get messages](../api/user-get-message.md)|[message](../resources/message.md)|Read the properties and relationships of a [message](../resources/message.md) object.|
|[List mailFolders](../api/user-list-mailfolders.md)|[mailFolder](../resources/mailfolder.md) collection|Get the mailFolders from the mailFolders navigation property.|
|[Create mailFolders](../api/user-post-mailfolders.md)|[mailFolder](../resources/mailfolder.md)|Create a new mailFolders object.|
|[Delete mailFolders](../api/user-delete-mailfolders.md)|None|Delete a [mailFolder](../resources/mailfolder.md) object.|
|[Update mailFolders](../api/user-update-mailfolders.md)|[mailFolder](../resources/mailfolder.md)|Update the properties of a mailFolders object.|
|[Get mailFolders](../api/user-get-mailfolder.md)|[mailFolder](../resources/mailfolder.md)|Read the properties and relationships of a [mailFolder](../resources/mailfolder.md) object.|
|[List calendar](../api/user-list-calendar.md)|[calendar](../resources/calendar.md) collection|Get the calendars from the calendar navigation property.|
|[Create calendar](../api/user-post-calendar.md)|[calendar](../resources/calendar.md)|Create a new calendar object.|
|[Delete calendar](../api/user-delete-calendar.md)|None|Delete a [calendar](../resources/calendar.md) object.|
|[Update calendar](../api/user-update-calendar.md)|[calendar](../resources/calendar.md)|Update the properties of a calendar object.|
|[Get calendar](../api/user-get-calendar.md)|[calendar](../resources/calendar.md)|Read the properties and relationships of a [calendar](../resources/calendar.md) object.|
|[List calendars](../api/user-list-calendars.md)|[calendar](../resources/calendar.md) collection|Get the calendars from the calendars navigation property.|
|[Create calendars](../api/user-post-calendars.md)|[calendar](../resources/calendar.md)|Create a new calendars object.|
|[Delete calendars](../api/user-delete-calendars.md)|None|Delete a [calendar](../resources/calendar.md) object.|
|[Update calendars](../api/user-update-calendars.md)|[calendar](../resources/calendar.md)|Update the properties of a calendars object.|
|[Get calendars](../api/user-get-calendar.md)|[calendar](../resources/calendar.md)|Read the properties and relationships of a [calendar](../resources/calendar.md) object.|
|[List calendarGroups](../api/user-list-calendargroups.md)|[calendarGroup](../resources/calendargroup.md) collection|Get the calendarGroups from the calendarGroups navigation property.|
|[Create calendarGroups](../api/user-post-calendargroups.md)|[calendarGroup](../resources/calendargroup.md)|Create a new calendarGroups object.|
|[Delete calendarGroups](../api/user-delete-calendargroups.md)|None|Delete a [calendarGroup](../resources/calendargroup.md) object.|
|[Update calendarGroups](../api/user-update-calendargroups.md)|[calendarGroup](../resources/calendargroup.md)|Update the properties of a calendarGroups object.|
|[Get calendarGroups](../api/user-get-calendargroup.md)|[calendarGroup](../resources/calendargroup.md)|Read the properties and relationships of a [calendarGroup](../resources/calendargroup.md) object.|
|[List calendarView](../api/user-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Create calendarView](../api/user-post-calendarview.md)|[event](../resources/event.md)|Create a new calendarView object.|
|[Delete calendarView](../api/user-delete-calendarview.md)|None|Delete an [event](../resources/event.md) object.|
|[Update calendarView](../api/user-update-calendarview.md)|[event](../resources/event.md)|Update the properties of a calendarView object.|
|[Get calendarView](../api/user-get-event.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|
|[List events](../api/user-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Create events](../api/user-post-events.md)|[event](../resources/event.md)|Create a new events object.|
|[Delete events](../api/user-delete-events.md)|None|Delete an [event](../resources/event.md) object.|
|[Update events](../api/user-update-events.md)|[event](../resources/event.md)|Update the properties of an events object.|
|[Get events](../api/user-get-event.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|
|[List people](../api/user-list-people.md)|[person](../resources/person.md) collection|Get the people from the people navigation property.|
|[Create people](../api/user-post-people.md)|[person](../resources/person.md)|Create a new people object.|
|[Delete people](../api/user-delete-people.md)|None|Delete a [person](../resources/person.md) object.|
|[Update people](../api/user-update-people.md)|[person](../resources/person.md)|Update the properties of a people object.|
|[Get people](../api/user-get-person.md)|[person](../resources/person.md)|Read the properties and relationships of a [person](../resources/person.md) object.|
|[List contacts](../api/user-list-contacts.md)|[contact](../resources/contact.md) collection|Get the contacts from the contacts navigation property.|
|[Create contacts](../api/user-post-contacts.md)|[contact](../resources/contact.md)|Create a new contacts object.|
|[Delete contacts](../api/user-delete-contacts.md)|None|Delete a [contact](../resources/contact.md) object.|
|[Update contacts](../api/user-update-contacts.md)|[contact](../resources/contact.md)|Update the properties of a contacts object.|
|[Get contacts](../api/user-get-contact.md)|[contact](../resources/contact.md)|Read the properties and relationships of a [contact](../resources/contact.md) object.|
|[List contactFolders](../api/user-list-contactfolders.md)|[contactFolder](../resources/contactfolder.md) collection|Get the contactFolders from the contactFolders navigation property.|
|[Create contactFolders](../api/user-post-contactfolders.md)|[contactFolder](../resources/contactfolder.md)|Create a new contactFolders object.|
|[Delete contactFolders](../api/user-delete-contactfolders.md)|None|Delete a [contactFolder](../resources/contactfolder.md) object.|
|[Update contactFolders](../api/user-update-contactfolders.md)|[contactFolder](../resources/contactfolder.md)|Update the properties of a contactFolders object.|
|[Get contactFolders](../api/user-get-contactfolder.md)|[contactFolder](../resources/contactfolder.md)|Read the properties and relationships of a [contactFolder](../resources/contactfolder.md) object.|
|[List inferenceClassification](../api/user-list-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md) collection|Get the inferenceClassifications from the inferenceClassification navigation property.|
|[Create inferenceClassification](../api/user-post-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md)|Create a new inferenceClassification object.|
|[Delete inferenceClassification](../api/user-delete-inferenceclassification.md)|None|Delete an [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Update inferenceClassification](../api/user-update-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md)|Update the properties of an inferenceClassification object.|
|[Get inferenceClassification](../api/user-get-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md)|Read the properties and relationships of an [inferenceClassification](../resources/inferenceclassification.md) object.|
|[List photo](../api/user-list-photo.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photo navigation property.|
|[Create photo](../api/user-post-photo.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photo object.|
|[Delete photo](../api/user-delete-photo.md)|None|Delete a [profilePhoto](../resources/profilephoto.md) object.|
|[Update photo](../api/user-update-photo.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a photo object.|
|[Get photo](../api/user-get-profilephoto.md)|[profilePhoto](../resources/profilephoto.md)|Read the properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[List photos](../api/user-list-photos.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photos navigation property.|
|[Create photos](../api/user-post-photos.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photos object.|
|[Delete photos](../api/user-delete-photos.md)|None|Delete a [profilePhoto](../resources/profilephoto.md) object.|
|[Update photos](../api/user-update-photos.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a photos object.|
|[Get photos](../api/user-get-profilephoto.md)|[profilePhoto](../resources/profilephoto.md)|Read the properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[List drive](../api/user-list-drive.md)|[drive](../resources/drive.md) collection|Get the drives from the drive navigation property.|
|[Create drive](../api/user-post-drive.md)|[drive](../resources/drive.md)|Create a new drive object.|
|[Delete drive](../api/user-delete-drive.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drive](../api/user-update-drive.md)|[drive](../resources/drive.md)|Update the properties of a drive object.|
|[Get drive](../api/user-get-drive.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List drives](../api/user-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Create drives](../api/user-post-drives.md)|[drive](../resources/drive.md)|Create a new drives object.|
|[Delete drives](../api/user-delete-drives.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drives](../api/user-update-drives.md)|[drive](../resources/drive.md)|Update the properties of a drives object.|
|[Get drives](../api/user-get-drive.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List followedSites](../api/user-list-followedsites.md)|[site](../resources/site.md) collection|Get the sites from the followedSites navigation property.|
|[Add followedSites](../api/user-post-followedsites.md)|[site](../resources/site.md)|Add followedSites by posting to the followedSites collection.|
|[Remove followedSites](../api/user-delete-followedsites.md)|None|Remove a [site](../resources/site.md) object.|
|[List extensions](../api/user-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/user-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[Delete extensions](../api/user-delete-extensions.md)|None|Delete an [extension](../resources/extension.md) object.|
|[Update extensions](../api/user-update-extensions.md)|[extension](../resources/extension.md)|Update the properties of an extensions object.|
|[Get extensions](../api/user-get-extension.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|
|[List managedDevices](../api/user-list-manageddevices.md)|[managedDevice](../resources/intune-manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Create managedDevices](../api/user-post-manageddevices.md)|[managedDevice](../resources/intune-manageddevice.md)|Create a new managedDevices object.|
|[Delete managedDevices](../api/user-delete-manageddevices.md)|None|Delete a [managedDevice](../resources/intune-manageddevice.md) object.|
|[Update managedDevices](../api/user-update-manageddevices.md)|[managedDevice](../resources/intune-manageddevice.md)|Update the properties of a managedDevices object.|
|[Get managedDevices](../api/user-get-manageddevice.md)|[managedDevice](../resources/intune-manageddevice.md)|Read the properties and relationships of a [managedDevice](../resources/intune-manageddevice.md) object.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/intune-managedappregistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Add managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/intune-managedappregistration.md)|Add managedAppRegistrations by posting to the managedAppRegistrations collection.|
|[Remove managedAppRegistrations](../api/user-delete-managedappregistrations.md)|None|Remove a [managedAppRegistration](../resources/intune-managedappregistration.md) object.|
|[List deviceManagementTroubleshootingEvents](../api/user-list-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md) collection|Get the deviceManagementTroubleshootingEvents from the deviceManagementTroubleshootingEvents navigation property.|
|[Create deviceManagementTroubleshootingEvents](../api/user-post-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md)|Create a new deviceManagementTroubleshootingEvents object.|
|[Delete deviceManagementTroubleshootingEvents](../api/user-delete-devicemanagementtroubleshootingevents.md)|None|Delete a [deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md) object.|
|[Update deviceManagementTroubleshootingEvents](../api/user-update-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md)|Update the properties of a deviceManagementTroubleshootingEvents object.|
|[Get deviceManagementTroubleshootingEvents](../api/user-get-devicemanagementtroubleshootingevent.md)|[deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md)|Read the properties and relationships of a [deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md) object.|
|[List decoratedProfile](../api/user-list-decoratedprofile.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|Get the DecoratedProfiles from the decoratedProfile navigation property.|
|[Add decoratedProfile](../api/user-post-decoratedprofile.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Add decoratedProfile by posting to the decoratedProfile collection.|
|[Remove decoratedProfile](../api/user-delete-decoratedprofile.md)|None|Remove a [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[List planner](../api/user-list-planner.md)|[plannerUser](../resources/planneruser.md) collection|Get the plannerUsers from the planner navigation property.|
|[Create planner](../api/user-post-planner.md)|[plannerUser](../resources/planneruser.md)|Create a new planner object.|
|[Delete planner](../api/user-delete-planner.md)|None|Delete a [plannerUser](../resources/planneruser.md) object.|
|[Update planner](../api/user-update-planner.md)|[plannerUser](../resources/planneruser.md)|Update the properties of a planner object.|
|[Get planner](../api/user-get-planneruser.md)|[plannerUser](../resources/planneruser.md)|Read the properties and relationships of a [plannerUser](../resources/planneruser.md) object.|
|[List insights](../api/user-list-insights.md)|[officeGraphInsights](../resources/officegraphinsights.md) collection|Get the officeGraphInsights from the insights navigation property.|
|[Create insights](../api/user-post-insights.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Create a new insights object.|
|[Delete insights](../api/user-delete-insights.md)|None|Delete an [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[Update insights](../api/user-update-insights.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Update the properties of an insights object.|
|[Get insights](../api/user-get-officegraphinsights.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Read the properties and relationships of an [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[List settings](../api/user-list-settings.md)|[userSettings](../resources/usersettings.md) collection|Get the userSettings from the settings navigation property.|
|[Create settings](../api/user-post-settings.md)|[userSettings](../resources/usersettings.md)|Create a new settings object.|
|[Delete settings](../api/user-delete-settings.md)|None|Delete a [userSettings](../resources/usersettings.md) object.|
|[Update settings](../api/user-update-settings.md)|[userSettings](../resources/usersettings.md)|Update the properties of a settings object.|
|[Get settings](../api/user-get-usersettings.md)|[userSettings](../resources/usersettings.md)|Read the properties and relationships of a [userSettings](../resources/usersettings.md) object.|
|[List onenote](../api/user-list-onenote.md)|[onenote](../resources/onenote.md) collection|Get the onenotes from the onenote navigation property.|
|[Create onenote](../api/user-post-onenote.md)|[onenote](../resources/onenote.md)|Create a new onenote object.|
|[Delete onenote](../api/user-delete-onenote.md)|None|Delete an [onenote](../resources/onenote.md) object.|
|[Update onenote](../api/user-update-onenote.md)|[onenote](../resources/onenote.md)|Update the properties of an onenote object.|
|[Get onenote](../api/user-get-onenote.md)|[onenote](../resources/onenote.md)|Read the properties and relationships of an [onenote](../resources/onenote.md) object.|
|[List activities](../api/user-list-activities.md)|[userActivity](../resources/projectrome-useractivity.md) collection|Get the userActivities from the activities navigation property.|
|[Create activities](../api/user-post-activities.md)|[userActivity](../resources/projectrome-useractivity.md)|Create a new activities object.|
|[Delete activities](../api/user-delete-activities.md)|None|Delete a [userActivity](../resources/projectrome-useractivity.md) object.|
|[Update activities](../api/user-update-activities.md)|[userActivity](../resources/projectrome-useractivity.md)|Update the properties of an activities object.|
|[Get activities](../api/user-get-useractivity.md)|[userActivity](../resources/projectrome-useractivity.md)|Read the properties and relationships of a [userActivity](../resources/projectrome-useractivity.md) object.|
|[List onlineMeetings](../api/user-list-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Create onlineMeetings](../api/user-post-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Create a new onlineMeetings object.|
|[Delete onlineMeetings](../api/user-delete-onlinemeetings.md)|None|Delete an [onlineMeeting](../resources/onlinemeeting.md) object.|
|[Update onlineMeetings](../api/user-update-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Update the properties of an onlineMeetings object.|
|[Get onlineMeetings](../api/user-get-onlinemeeting.md)|[onlineMeeting](../resources/onlinemeeting.md)|Read the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.|
|[List joinedTeams](../api/user-list-joinedteams.md)|[team](../resources/team.md) collection|Get the teams from the joinedTeams navigation property.|
|[Create joinedTeams](../api/user-post-joinedteams.md)|[team](../resources/team.md)|Create a new joinedTeams object.|
|[Delete joinedTeams](../api/user-delete-joinedteams.md)|None|Delete a [team](../resources/team.md) object.|
|[Update joinedTeams](../api/user-update-joinedteams.md)|[team](../resources/team.md)|Update the properties of a joinedTeams object.|
|[Get joinedTeams](../api/user-get-team.md)|[team](../resources/team.md)|Read the properties and relationships of a [team](../resources/team.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aboutMe|String|**TODO: Add Description**|
|accountEnabled|Boolean|**TODO: Add Description**|
|ageGroup|String|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|birthday|DateTimeOffset|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|consentProvidedForMinor|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|creationType|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|department|String|**TODO: Add Description**|
|deviceEnrollmentLimit|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|employeeId|String|**TODO: Add Description**|
|faxNumber|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|hireDate|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|identities|[objectIdentity](../resources/objectidentity.md) collection|**TODO: Add Description**|
|imAddresses|String collection|**TODO: Add Description**|
|interests|String collection|**TODO: Add Description**|
|isResourceAccount|Boolean|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|lastPasswordChangeDateTime|DateTimeOffset|**TODO: Add Description**|
|legalAgeGroupClassification|String|**TODO: Add Description**|
|licenseAssignmentStates|[licenseAssignmentState](../resources/licenseassignmentstate.md) collection|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailboxSettings|[mailboxSettings](../resources/mailboxsettings.md)|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|mySite|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|onPremisesDistinguishedName|String|**TODO: Add Description**|
|onPremisesDomainName|String|**TODO: Add Description**|
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description**|
|onPremisesImmutableId|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSamAccountName|String|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|onPremisesUserPrincipalName|String|**TODO: Add Description**|
|otherMails|String collection|**TODO: Add Description**|
|passwordPolicies|String|**TODO: Add Description**|
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description**|
|pastProjects|String collection|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|preferredName|String|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|responsibilities|String collection|**TODO: Add Description**|
|schools|String collection|**TODO: Add Description**|
|showInAddressList|Boolean|**TODO: Add Description**|
|signInSessionsValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|skills|String collection|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|streetAddress|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|usageLocation|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userType|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[userActivity](../resources/projectrome-useractivity.md) collection|**TODO: Add Description**|
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|calendar|[calendar](../resources/calendar.md)|**TODO: Add Description**|
|calendarGroups|[calendarGroup](../resources/calendargroup.md) collection|**TODO: Add Description**|
|calendars|[calendar](../resources/calendar.md) collection|**TODO: Add Description**|
|calendarView|[event](../resources/event.md) collection|**TODO: Add Description**|
|contactFolders|[contactFolder](../resources/contactfolder.md) collection|**TODO: Add Description**|
|contacts|[contact](../resources/contact.md) collection|**TODO: Add Description**|
|createdObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|decoratedProfile|[DecoratedProfile](../resources/decoratedprofile.md)|**TODO: Add Description**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-devicemanagementtroubleshootingevent.md) collection|**TODO: Add Description**|
|directReports|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|drive|[drive](../resources/drive.md)|**TODO: Add Description**|
|drives|[drive](../resources/drive.md) collection|**TODO: Add Description**|
|events|[event](../resources/event.md) collection|**TODO: Add Description**|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|followedSites|[site](../resources/site.md) collection|**TODO: Add Description**|
|inferenceClassification|[inferenceClassification](../resources/inferenceclassification.md)|**TODO: Add Description**|
|insights|[officeGraphInsights](../resources/officegraphinsights.md)|**TODO: Add Description**|
|joinedTeams|[team](../resources/team.md) collection|**TODO: Add Description**|
|licenseDetails|[licenseDetails](../resources/licensedetails.md) collection|**TODO: Add Description**|
|mailFolders|[mailFolder](../resources/mailfolder.md) collection|**TODO: Add Description**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-managedappregistration.md) collection|**TODO: Add Description**|
|managedDevices|[managedDevice](../resources/intune-manageddevice.md) collection|**TODO: Add Description**|
|manager|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|messages|[message](../resources/message.md) collection|**TODO: Add Description**|
|oauth2PermissionGrants|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|**TODO: Add Description**|
|onenote|[onenote](../resources/onenote.md)|**TODO: Add Description**|
|onlineMeetings|[onlineMeeting](../resources/onlinemeeting.md) collection|**TODO: Add Description**|
|outlook|[outlookUser](../resources/outlookuser.md)|**TODO: Add Description**|
|ownedDevices|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|ownedObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|people|[person](../resources/person.md) collection|**TODO: Add Description**|
|photo|[profilePhoto](../resources/profilephoto.md)|**TODO: Add Description**|
|photos|[profilePhoto](../resources/profilephoto.md) collection|**TODO: Add Description**|
|planner|[plannerUser](../resources/planneruser.md)|**TODO: Add Description**|
|registeredDevices|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|settings|[userSettings](../resources/usersettings.md)|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "accountEnabled": "Boolean",
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "creationType": "String",
  "department": "String",
  "displayName": "String",
  "employeeId": "String",
  "faxNumber": "String",
  "givenName": "String",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "isResourceAccount": "Boolean",
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState"
    }
  ],
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesDomainName": "String",
  "onPremisesSamAccountName": "String",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "postalCode": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "showInAddressList": "Boolean",
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "mailboxSettings": {
    "@odata.type": "microsoft.graph.mailboxSettings"
  },
  "deviceEnrollmentLimit": "Integer",
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

