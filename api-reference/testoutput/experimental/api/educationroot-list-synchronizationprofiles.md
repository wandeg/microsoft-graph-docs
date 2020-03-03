---
title: "List synchronizationProfiles"
description: "Get the educationSynchronizationProfiles from the synchronizationProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List synchronizationProfiles

Namespace: microsoft.graph

Get the educationSynchronizationProfiles from the synchronizationProfiles navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/synchronizationProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/synchronizationProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsynchronizationprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
      "id": "0926f8a0-f8a0-0926-a0f8-2609a0f82609",
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
  ]
}
```

