---
title: "mobileApp resource type"
description: "An abstract class containing the base properties for Intune mobile apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mobileApp resource type

An abstract class containing the base properties for Intune mobile apps.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileApp](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileApp.md)|Read properties and relationships of the [mobileApp](../resources/mobileapp.md) object.|
|[assign](../api/intune-apps-mobileapp-assign.md)|None||
|[updateRelationships](../api/intune-apps-mobileapp-updaterelationships.md)|None||
|[getRelatedAppStates](../api/intune-apps-mobileapp-getrelatedappstates.md)|[mobileAppRelationshipState](../resources/intune-apps-mobileAppRelationshipState.md) collection||
|[getMobileAppCount](../api/intune-apps-mobileapp-getmobileappcount.md)|Int64||
|[getTopMobileApps](../api/intune-apps-mobileapp-gettopmobileapps.md)|[mobileApp](../resources/intune-apps-mobileApp.md) collection||
|[hasPayloadLinks](../api/intune-apps-mobileapp-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/hasPayloadLinkResultItem.md) collection||
|[List categories](../api/intune-apps-mobileapp-list-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/intune-apps-mobileapp-post-categories.md)|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/intune-apps-mobileapp-list-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/intune-apps-mobileapp-post-assignments.md)|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/intune-apps-mobileapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/intune-apps-mobileapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/intune-apps-mobileapp-list-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/intune-apps-mobileapp-post-userstatuses.md)|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List relationships](../api/intune-apps-mobileapp-list-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Add relationships](../api/intune-apps-mobileapp-post-relationships.md)|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md)|Add relationships by posting to the relationships collection.|
|[List mobileApps](../api/intune-apps-deviceappmanagement-list-mobileapps.md)|[mobileApp](../resources/intune-apps-mobileApp.md) collection|Get the mobileApps from the mobileApps navigation property.|
|[Add mobileApps](../api/intune-apps-deviceappmanagement-post-mobileapps.md)|[mobileApp](../resources/intune-apps-mobileApp.md)|Add mobileApps by posting to the mobileApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the app was created.|
|dependentAppCount|Int32|The total number of dependencies the child app has.|
|description|String|The description of the app.|
|developer|String|The developer of the app.|
|displayName|String|The admin provided or imported title of the app.|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url.|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group.|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin.|
|largeIcon|[mimeContent](../resources/intune-apps-mimeContent.md)|The large icon, to be displayed in the app details and used for upload of the icon.|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified.|
|notes|String|Notes for the app.|
|owner|String|The owner of the app.|
|privacyInformationUrl|String|The privacy statement Url.|
|publisher|String|The publisher of the app.|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app.|
|uploadState|Int32|The upload state.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileAppAssignment.md) collection|The list of group assignments for this mobile app.|
|categories|[mobileAppCategory](../resources/intune-apps-mobileAppCategory.md) collection|The list of categories for this app.|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileAppInstallStatus.md) collection|The list of installation states for this mobile app.|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileAppInstallSummary.md)|Mobile App Install Summary.|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileAppRelationship.md) collection|List of relationships for this mobile app.|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userAppInstallStatus.md) collection|The list of installation states for this mobile app.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024
}
```

