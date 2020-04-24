---
title: "Update educationSynchronizationProfile"
description: "Update the properties of an educationSynchronizationProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update educationSynchronizationProfile

Namespace: microsoft.graph

Update the properties of an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/synchronizationProfiles/{educationSynchronizationProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|dataProvider|[educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)|**TODO: Add Description**|
|identitySynchronizationConfiguration|[educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md)|**TODO: Add Description**|
|licensesToAssign|[educationSynchronizationLicenseAssignment](../resources/educationsynchronizationlicenseassignment.md) collection|**TODO: Add Description**|
|state|educationSynchronizationProfileState|**TODO: Add Description**. Possible values are: `deleting`, `deletionFailed`, `provisioningFailed`, `provisioned`, `provisioning`, `unknownFutureValue`.|
|handleSpecialCharacterConstraint|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_educationsynchronizationprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}
Content-Type: application/json
Content-length: 628

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "displayName": "Display Name value",
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
        "Sku Ids value"
      ]
    }
  ],
  "state": "String",
  "handleSpecialCharacterConstraint": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "id": "2380a6b9-a6b9-2380-b9a6-8023b9a68023",
  "displayName": "Display Name value",
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
        "Sku Ids value"
      ]
    }
  ],
  "state": "String",
  "handleSpecialCharacterConstraint": true
}
```

