---
title: "educationSynchronizationProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationSynchronizationProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSynchronizationProfile](../api/educationsynchronizationprofile-get.md)|[educationSynchronizationProfile](../resources/educationSynchronizationProfile.md)|Read properties and relationships of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.|
|[Delete educationSynchronizationProfile](../api/educationsynchronizationprofile-delete.md)|None|Deletes a [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).|
|[Update educationSynchronizationProfile](../api/educationsynchronizationprofile-update.md)|[educationSynchronizationProfile](../resources/educationSynchronizationProfile.md)|Update the properties of a [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.|
|[resume](../api/educationsynchronizationprofile-resume.md)|None||
|[pause](../api/educationsynchronizationprofile-pause.md)|None||
|[reset](../api/educationsynchronizationprofile-reset.md)|None||
|[start](../api/educationsynchronizationprofile-start.md)|[educationFileSynchronizationVerificationMessage](../resources/educationFileSynchronizationVerificationMessage.md) collection||
|[uploadUrl](../api/educationsynchronizationprofile-uploadurl.md)|String||
|[List errors](../api/educationsynchronizationprofile-list-errors.md)|[educationSynchronizationError](../resources/educationSynchronizationError.md) collection|Get the educationSynchronizationErrors from the errors navigation property.|
|[Add errors](../api/educationsynchronizationprofile-post-errors.md)|[educationSynchronizationError](../resources/educationSynchronizationError.md)|Add errors by posting to the errors collection.|
|[Get educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-get.md)|[educationSynchronizationProfileStatus](../resources/educationSynchronizationProfileStatus.md)|Read properties and relationships of the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|
|[List synchronizationProfiles](../api/educationroot-list-synchronizationprofiles.md)|[educationSynchronizationProfile](../resources/educationSynchronizationProfile.md) collection|Get the educationSynchronizationProfiles from the synchronizationProfiles navigation property.|
|[Add synchronizationProfiles](../api/educationroot-post-synchronizationprofiles.md)|[educationSynchronizationProfile](../resources/educationSynchronizationProfile.md)|Add synchronizationProfiles by posting to the synchronizationProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataProvider|[educationSynchronizationDataProvider](../resources/educationSynchronizationDataProvider.md)||
|displayName|String||
|handleSpecialCharacterConstraint|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|identitySynchronizationConfiguration|[educationIdentitySynchronizationConfiguration](../resources/educationIdentitySynchronizationConfiguration.md)||
|licensesToAssign|[educationSynchronizationLicenseAssignment](../resources/educationSynchronizationLicenseAssignment.md) collection||
|state|Enumeration|. Possible values are: `deleting`, `deletionFailed`, `provisioningFailed`, `provisioned`, `provisioning`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|errors|[educationSynchronizationError](../resources/educationSynchronizationError.md) collection||
|profileStatus|[educationSynchronizationProfileStatus](../resources/educationSynchronizationProfileStatus.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
      "appliesTo": "String",
      "skuIds": [
        "String"
      ]
    }
  ],
  "state": "String",
  "handleSpecialCharacterConstraint": true
}
```

