---
title: "educationSynchronizationProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSynchronizationProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationSynchronizationProfiles](../api/educationsynchronizationprofile-list.md)|[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) collection|List properties and relationships of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects.|
|[Get educationSynchronizationProfile](../api/educationsynchronizationprofile-get.md)|[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)|Read properties and relationships of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.|
|[Create educationSynchronizationProfile](../api/educationsynchronizationprofile-create.md)|[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)|Create a new [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.|
|[Delete educationSynchronizationProfile](../api/educationsynchronizationprofile-delete.md)|None|Deletes a [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).|
|[Update educationSynchronizationProfile](../api/educationsynchronizationprofile-update.md)|[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)|Update the properties of a [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.|
|[resume](../api/educationsynchronizationprofile-resume.md)|None||
|[pause](../api/educationsynchronizationprofile-pause.md)|None||
|[reset](../api/educationsynchronizationprofile-reset.md)|None||
|[start](../api/educationsynchronizationprofile-start.md)|[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) collection||
|[uploadUrl](../api/educationsynchronizationprofile-uploadurl.md)|String||
|[List errors](../api/educationsynchronizationprofile-list-errors.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md) collection|Get the educationSynchronizationErrors from the errors navigation property.|
|[Add errors](../api/educationsynchronizationprofile-post-errors.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Add errors by posting to the errors collection.|
|[Get educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-get.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Read properties and relationships of the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|
|[List synchronizationProfiles](../api/educationroot-list-synchronizationprofiles.md)|[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) collection|Get the educationSynchronizationProfiles from the synchronizationProfiles navigation property.|
|[Add synchronizationProfiles](../api/educationroot-post-synchronizationprofiles.md)|[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)|Add synchronizationProfiles by posting to the synchronizationProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataProvider|[educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)||
|displayName|String||
|handleSpecialCharacterConstraint|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|identitySynchronizationConfiguration|[educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md)||
|licensesToAssign|[educationSynchronizationLicenseAssignment](../resources/educationsynchronizationlicenseassignment.md) collection||
|state|Enumeration|. Possible values are: `deleting`, `deletionFailed`, `provisioningFailed`, `provisioned`, `provisioning`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|errors|[educationSynchronizationError](../resources/educationsynchronizationerror.md) collection||
|profileStatus|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)||

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

