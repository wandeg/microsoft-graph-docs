---
title: "List synchronizationProfiles"
description: "Get the educationSynchronizationProfiles from the synchronizationProfiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List synchronizationProfiles

Namespace: microsoft.graph

Get the educationSynchronizationProfiles from the synchronizationProfiles navigation property.

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
GET /education/synchronizationProfiles
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsynchronizationprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

