---
title: "List azureADUserFeatureUsages"
description: "Get a list of the azureADUserFeatureUsage objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List azureADUserFeatureUsages
Namespace: microsoft.graph

Get a list of the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.azureADUserFeatureUsage not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_azureaduserfeatureusage"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.azureADUserFeatureUsage not found
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.azureaduserfeatureusage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.azureADUserFeatureUsage",
      "id": "12dd51df-51df-12dd-df51-dd12df51dd12",
      "lastUpdatedDateTime": "String (timestamp)",
      "userId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "licenseRecommended": "String",
      "licenseAssigned": "String",
      "featureUsageDetails": [
        {
          "@odata.type": "microsoft.graph.featureUsageDetail"
        }
      ]
    }
  ]
}
```

