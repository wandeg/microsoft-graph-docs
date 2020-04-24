---
title: "mobileApp resource type"
description: "An abstract class containing the base properties for Intune mobile apps."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileApp resource type


Namespace: microsoft.graph

An abstract class containing the base properties for Intune mobile apps.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileApp](../api/mobileapp-get.md)|[mobileApp](../resources/mobileapp.md)|Read the properties and relationships of a [mobileApp](../resources/mobileapp.md) object.|
|[assign](../api/mobileapp-assign.md)|None|**TODO: Add Description**|
|[updateRelationships](../api/mobileapp-updaterelationships.md)|None|**TODO: Add Description**|
|[getRelatedAppStates](../api/mobileapp-getrelatedappstates.md)|[mobileAppRelationshipState](../resources/mobileapprelationshipstate.md) collection|**TODO: Add Description**|
|[getMobileAppCount](../api/mobileapp-getmobileappcount.md)|Int64|**TODO: Add Description**|
|[getTopMobileApps](../api/mobileapp-gettopmobileapps.md)|[mobileApp](../resources/mobileapp.md) collection|**TODO: Add Description**|
|[hasPayloadLinks](../api/mobileapp-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[List categories](../api/mobileapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Add categories](../api/mobileapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Add categories by posting to the categories collection.|
|[Remove categories](../api/mobileapp-delete-categories.md)|None|Remove a [mobileAppCategory](../resources/mobileappcategory.md) object.|
|[List assignments](../api/mobileapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Create assignments](../api/mobileapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/mobileapp-delete-assignments.md)|None|Delete an [mobileAppAssignment](../resources/mobileappassignment.md) object.|
|[Update assignments](../api/mobileapp-update-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Update the properties of an assignments object.|
|[Get mobileAppAssignment](../api/mobileappassignment-get.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Read the properties and relationships of a [mobileAppAssignment](../resources/mobileappassignment.md) object.|
|[List installSummary](../api/mobileapp-list-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md) collection|Get the mobileAppInstallSummaries from the installSummary navigation property.|
|[Create installSummary](../api/mobileapp-post-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Create a new installSummary object.|
|[Delete installSummary](../api/mobileapp-delete-installsummary.md)|None|Delete an [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Update installSummary](../api/mobileapp-update-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Update the properties of an installSummary object.|
|[Get mobileAppInstallSummary](../api/mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Read the properties and relationships of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List deviceStatuses](../api/mobileapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/mobileapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/mobileapp-delete-devicestatuses.md)|None|Delete a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[Update deviceStatuses](../api/mobileapp-update-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Update the properties of a deviceStatuses object.|
|[Get mobileAppInstallStatus](../api/mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Read the properties and relationships of a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[List userStatuses](../api/mobileapp-list-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|Get the userAppInstallStatus from the userStatuses navigation property.|
|[Create userStatuses](../api/mobileapp-post-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Create a new userStatuses object.|
|[Delete userStatuses](../api/mobileapp-delete-userstatuses.md)|None|Delete a [userAppInstallStatus](../resources/userappinstallstatus.md) object.|
|[Update userStatuses](../api/mobileapp-update-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Update the properties of a userStatuses object.|
|[Get userAppInstallStatus](../api/userappinstallstatus-get.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Read the properties and relationships of a [userAppInstallStatus](../resources/userappinstallstatus.md) object.|
|[List relationships](../api/mobileapp-list-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|Get the mobileAppRelationships from the relationships navigation property.|
|[Create relationships](../api/mobileapp-post-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md)|Create a new relationships object.|
|[Delete relationships](../api/mobileapp-delete-relationships.md)|None|Delete a [mobileAppRelationship](../resources/mobileapprelationship.md) object.|
|[Update relationships](../api/mobileapp-update-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md)|Update the properties of a relationships object.|
|[Get mobileAppRelationship](../api/mobileapprelationship-get.md)|[mobileAppRelationship](../resources/mobileapprelationship.md)|Read the properties and relationships of a [mobileAppRelationship](../resources/mobileapprelationship.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the app was created.|
|dependentAppCount|Int32|The total number of dependencies the child app has.|
|description|String|The description of the app.|
|developer|String|The developer of the app.|
|displayName|String|The admin provided or imported title of the app.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url.|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group.|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin.|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon.|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified.|
|notes|String|Notes for the app.|
|owner|String|The owner of the app.|
|privacyInformationUrl|String|The privacy statement Url.|
|publisher|String|The publisher of the app.|
|publishingState|mobileAppPublishingState|The publishing state for the app. The app cannot be assigned unless the app is published. Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app.|
|uploadState|Int32|The upload state.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app.|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app.|
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|The list of installation states for this mobile app.|
|installSummary|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Mobile App Install Summary.|
|relationships|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|List of relationships for this mobile app.|
|userStatuses|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|The list of installation states for this mobile app.|

## JSON representation
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

