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
|[List users](../api/user-list.md)|[user](../resources/user.md) collection|List properties and relationships of the [user](../resources/user.md) objects.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Create user](../api/user-post-users.md)|[user](../resources/user.md)|Create a new [user](../resources/user.md) object.|
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
|[revokeSignInSessions](../api/user-revokesigninsessions.md)|Boolean||
|[findMeetingTimes](../api/user-findmeetingtimes.md)|[meetingTimeSuggestionsResult](../resources/meetingTimeSuggestionsResult.md)||
|[sendMail](../api/user-sendmail.md)|None||
|[getMailTips](../api/user-getmailtips.md)|[mailTips](../resources/mailTips.md) collection||
|[translateExchangeIds](../api/user-translateexchangeids.md)|[convertIdResult](../resources/convertIdResult.md) collection||
|[removeAllDevicesFromManagement](../api/user-removealldevicesfrommanagement.md)|None||
|[getManagedAppDiagnosticStatuses](../api/user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/managedAppDiagnosticStatus.md) collection||
|[getManagedAppPolicies](../api/user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/managedAppPolicy.md) collection||
|[wipeManagedAppRegistrationsByDeviceTag](../api/user-wipemanagedappregistrationsbydevicetag.md)|None||
|[exportPersonalData](../api/user-exportpersonaldata.md)|None||
|[List ownedDevices](../api/user-list-owneddevices.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the ownedDevices navigation property.|
|[Create ownedDevices](../api/user-post-owneddevices.md)|[directoryObject](../resources/directoryObject.md)|Create ownedDevices by posting to the ownedDevices collection.|
|[List registeredDevices](../api/user-list-registereddevices.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the registeredDevices navigation property.|
|[Create registeredDevices](../api/user-post-registereddevices.md)|[directoryObject](../resources/directoryObject.md)|Create registeredDevices by posting to the registeredDevices collection.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryObject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[List directReports](../api/user-list-directreports.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the directReports navigation property.|
|[Create directReports](../api/user-post-directreports.md)|[directoryObject](../resources/directoryObject.md)|Create directReports by posting to the directReports collection.|
|[List memberOf](../api/user-list-memberof.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Create memberOf](../api/user-post-memberof.md)|[directoryObject](../resources/directoryObject.md)|Create memberOf by posting to the memberOf collection.|
|[List createdObjects](../api/user-list-createdobjects.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the createdObjects navigation property.|
|[Create createdObjects](../api/user-post-createdobjects.md)|[directoryObject](../resources/directoryObject.md)|Create createdObjects by posting to the createdObjects collection.|
|[List ownedObjects](../api/user-list-ownedobjects.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the ownedObjects navigation property.|
|[Create ownedObjects](../api/user-post-ownedobjects.md)|[directoryObject](../resources/directoryObject.md)|Create ownedObjects by posting to the ownedObjects collection.|
|[List licenseDetails](../api/user-list-licensedetails.md)|[licenseDetails](../resources/licenseDetails.md) collection|Get the licenseDetailses from the licenseDetails navigation property.|
|[Add licenseDetails](../api/user-post-licensedetails.md)|[licenseDetails](../resources/licenseDetails.md)|Add licenseDetails by posting to the licenseDetails collection.|
|[List transitiveMemberOf](../api/user-list-transitivememberof.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Create transitiveMemberOf](../api/user-post-transitivememberof.md)|[directoryObject](../resources/directoryObject.md)|Create transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Get outlookUser](../api/outlookuser-get.md)|[outlookUser](../resources/outlookUser.md)|Read properties and relationships of the [outlookUser](../resources/outlookuser.md) object.|
|[List messages](../api/user-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Add messages](../api/user-post-messages.md)|[message](../resources/message.md)|Add messages by posting to the messages collection.|
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
|[List extensions](../api/user-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/user-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List managedDevices](../api/user-list-manageddevices.md)|[managedDevice](../resources/managedDevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Add managedDevices](../api/user-post-manageddevices.md)|[managedDevice](../resources/managedDevice.md)|Add managedDevices by posting to the managedDevices collection.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/managedAppRegistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Create managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/managedAppRegistration.md)|Create managedAppRegistrations by posting to the managedAppRegistrations collection.|
|[List deviceManagementTroubleshootingEvents](../api/user-list-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md) collection|Get the deviceManagementTroubleshootingEvents from the deviceManagementTroubleshootingEvents navigation property.|
|[Add deviceManagementTroubleshootingEvents](../api/user-post-devicemanagementtroubleshootingevents.md)|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md)|Add deviceManagementTroubleshootingEvents by posting to the deviceManagementTroubleshootingEvents collection.|
|[Get plannerUser](../api/planneruser-get.md)|[plannerUser](../resources/plannerUser.md)|Read properties and relationships of the [plannerUser](../resources/planneruser.md) object.|
|[Get officeGraphInsights](../api/officegraphinsights-get.md)|[officeGraphInsights](../resources/officeGraphInsights.md)|Read properties and relationships of the [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[Get userSettings](../api/usersettings-get.md)|[userSettings](../resources/userSettings.md)|Read properties and relationships of the [userSettings](../resources/usersettings.md) object.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of the [onenote](../resources/onenote.md) object.|
|[List activities](../api/user-list-activities.md)|[userActivity](../resources/userActivity.md) collection|Get the userActivities from the activities navigation property.|
|[Add activities](../api/user-post-activities.md)|[userActivity](../resources/userActivity.md)|Add activities by posting to the activities collection.|
|[List onlineMeetings](../api/user-list-onlinemeetings.md)|[onlineMeeting](../resources/onlineMeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Add onlineMeetings](../api/user-post-onlinemeetings.md)|[onlineMeeting](../resources/onlineMeeting.md)|Add onlineMeetings by posting to the onlineMeetings collection.|
|[List joinedTeams](../api/user-list-joinedteams.md)|[group](../resources/group.md) collection|Get the groups from the joinedTeams navigation property.|
|[Add joinedTeams](../api/user-post-joinedteams.md)|[group](../resources/group.md)|Add joinedTeams by posting to the joinedTeams collection.|

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
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|department|String||
|deviceEnrollmentLimit|Int32|The limit on the maximum number of devices that the user is permitted to enroll. Allowed values are 5 or 1000.|
|displayName|String||
|employeeId|String||
|faxNumber|String||
|givenName|String||
|hireDate|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
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
|preferredLanguage|String||
|preferredName|String||
|provisionedPlans|[provisionedPlan](../resources/provisionedPlan.md) collection||
|proxyAddresses|String collection||
|responsibilities|String collection||
|schools|String collection||
|showInAddressList|Boolean||
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
|calendar|[calendar](../resources/calendar.md)||
|calendarGroups|[calendarGroup](../resources/calendarGroup.md) collection||
|calendars|[calendar](../resources/calendar.md) collection||
|calendarView|[event](../resources/event.md) collection||
|contactFolders|[contactFolder](../resources/contactFolder.md) collection||
|contacts|[contact](../resources/contact.md) collection||
|createdObjects|[directoryObject](../resources/directoryObject.md) collection||
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/deviceManagementTroubleshootingEvent.md) collection|The list of troubleshooting events for this user.|
|directReports|[directoryObject](../resources/directoryObject.md) collection||
|drive|[drive](../resources/drive.md)||
|drives|[drive](../resources/drive.md) collection||
|events|[event](../resources/event.md) collection||
|extensions|[extension](../resources/extension.md) collection||
|inferenceClassification|[inferenceClassification](../resources/inferenceClassification.md)||
|insights|[officeGraphInsights](../resources/officeGraphInsights.md)||
|joinedTeams|[group](../resources/group.md) collection||
|licenseDetails|[licenseDetails](../resources/licenseDetails.md) collection||
|mailFolders|[mailFolder](../resources/mailFolder.md) collection||
|managedAppRegistrations|[managedAppRegistration](../resources/managedAppRegistration.md) collection|Zero or more managed app registrations that belong to the user.|
|managedDevices|[managedDevice](../resources/managedDevice.md) collection|The managed devices associated with the user.|
|manager|[directoryObject](../resources/directoryObject.md)||
|memberOf|[directoryObject](../resources/directoryObject.md) collection||
|messages|[message](../resources/message.md) collection||
|onenote|[onenote](../resources/onenote.md)||
|onlineMeetings|[onlineMeeting](../resources/onlineMeeting.md) collection||
|outlook|[outlookUser](../resources/outlookUser.md)||
|ownedDevices|[directoryObject](../resources/directoryObject.md) collection||
|ownedObjects|[directoryObject](../resources/directoryObject.md) collection||
|people|[person](../resources/person.md) collection||
|photo|[profilePhoto](../resources/profilePhoto.md)||
|photos|[profilePhoto](../resources/profilePhoto.md) collection||
|planner|[plannerUser](../resources/plannerUser.md)||
|registeredDevices|[directoryObject](../resources/directoryObject.md) collection||
|settings|[userSettings](../resources/userSettings.md)||
|transitiveMemberOf|[directoryObject](../resources/directoryObject.md) collection||

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
  "accountEnabled": true,
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
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
  "department": "String",
  "displayName": "String",
  "employeeId": "String",
  "faxNumber": "String",
  "givenName": "String",
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
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
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
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
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

