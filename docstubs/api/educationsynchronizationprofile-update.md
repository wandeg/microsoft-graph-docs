---
title: "Update educationSynchronizationProfile"
description: "Update the properties of a educationSynchronizationProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationSynchronizationProfile

Namespace: microsoft.graph

Update the properties of a [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|dataProvider|[educationSynchronizationDataProvider](../resources/educationsynchronizationdataprovider.md)||
|identitySynchronizationConfiguration|[educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md)||
|licensesToAssign|[educationSynchronizationLicenseAssignment](../resources/educationsynchronizationlicenseassignment.md) collection||
|state|Enumeration| Possible values are: `deleting`, `deletionFailed`, `provisioningFailed`, `provisioned`, `provisioning`, `unknownFutureValue`.|
|handleSpecialCharacterConstraint|Boolean||



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
Content-type: application/json
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "id": "da345fa9-5fa9-da34-a95f-34daa95f34da",
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

