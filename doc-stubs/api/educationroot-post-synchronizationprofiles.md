---
title: "Create synchronizationProfiles"
description: "Create a new synchronizationProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create synchronizationProfiles

Namespace: microsoft.graph

Create a new synchronizationProfiles object.

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
POST /education/synchronizationProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationsynchronizationprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-Type: application/json
Content-length: 537

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsynchronizationprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "id": "a730ff27-ff27-a730-27ff-30a727ff30a7",
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

