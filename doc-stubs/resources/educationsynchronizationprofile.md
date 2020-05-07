---
title: "educationSynchronizationProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationSynchronizationProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[resume](../api/educationsynchronizationprofile-resume.md)|None|**TODO: Add Description**|
|[pause](../api/educationsynchronizationprofile-pause.md)|None|**TODO: Add Description**|
|[reset](../api/educationsynchronizationprofile-reset.md)|None|**TODO: Add Description**|
|[start](../api/educationsynchronizationprofile-start.md)|[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) collection|**TODO: Add Description**|
|[uploadUrl](../api/educationsynchronizationprofile-uploadurl.md)|String|**TODO: Add Description**|
|[List errors](../api/educationsynchronizationprofile-list-errors.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md) collection|Get the educationSynchronizationErrors from the errors navigation property.|
|[Create errors](../api/educationsynchronizationprofile-post-errors.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Create a new errors object.|
|[Delete errors](../api/educationsynchronizationprofile-delete-errors.md)|None|Delete an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|
|[Update errors](../api/educationsynchronizationprofile-update-errors.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Update the properties of an errors object.|
|[Get educationSynchronizationError](../api/educationsynchronizationerror-get.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Read the properties and relationships of an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|
|[List profileStatus](../api/educationsynchronizationprofile-list-profilestatus.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) collection|Get the educationSynchronizationProfileStatus from the profileStatus navigation property.|
|[Create profileStatus](../api/educationsynchronizationprofile-post-profilestatus.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Create a new profileStatus object.|
|[Delete profileStatus](../api/educationsynchronizationprofile-delete-profilestatus.md)|None|Delete a [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|
|[Update profileStatus](../api/educationsynchronizationprofile-update-profilestatus.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Update the properties of a profileStatus object.|
|[Get educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-get.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Read the properties and relationships of an [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataProvider|[educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|handleSpecialCharacterConstraint|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|identitySynchronizationConfiguration|[educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md)|**TODO: Add Description**|
|licensesToAssign|[educationSynchronizationLicenseAssignment](../resources/educationsynchronizationlicenseassignment.md) collection|**TODO: Add Description**|
|state|educationSynchronizationProfileState|**TODO: Add Description**. Possible values are: `deleting`, `deletionFailed`, `provisioningFailed`, `provisioned`, `provisioning`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|errors|[educationSynchronizationError](../resources/educationsynchronizationerror.md) collection|**TODO: Add Description**|
|profileStatus|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationSynchronizationDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "state": "String",
  "handleSpecialCharacterConstraint": "Boolean"
}
```

