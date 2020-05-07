---
title: "mobileApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
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
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|dependentAppCount|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|developer|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|informationUrl|String|**TODO: Add Description**|
|isAssigned|Boolean|**TODO: Add Description**|
|isFeatured|Boolean|**TODO: Add Description**|
|largeIcon|[mimeContent](../resources/mimecontent.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|notes|String|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|privacyInformationUrl|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|publishingState|mobileAppPublishingState|**TODO: Add Description**. Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|uploadState|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|**TODO: Add Description**|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|**TODO: Add Description**|
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|**TODO: Add Description**|
|installSummary|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|**TODO: Add Description**|
|relationships|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|**TODO: Add Description**|
|userStatuses|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": "Boolean",
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": "Integer",
  "publishingState": "String",
  "isAssigned": "Boolean",
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": "Integer"
}
```

