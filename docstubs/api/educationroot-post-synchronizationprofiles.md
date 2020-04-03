---
title: "Add synchronizationProfiles"
description: "Add synchronizationProfiles by posting to the synchronizationProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add synchronizationProfiles

Namespace: microsoft.graph

Add synchronizationProfiles by posting to the synchronizationProfiles collection.

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
POST /education/synchronizationProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationsynchronizationprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsynchronizationprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "id": "38548bd1-8bd1-3854-d18b-5438d18b5438",
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

