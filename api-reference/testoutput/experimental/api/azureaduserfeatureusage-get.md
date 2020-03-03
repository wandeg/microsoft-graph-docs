---
title: "Get azureADUserFeatureUsage"
description: "Read properties and relationships of the azureADUserFeatureUsage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get azureADUserFeatureUsage

Namespace: microsoft.graph

Read properties and relationships of the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object.

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
GET ** Entity URI for microsoft.graph.azureADUserFeatureUsage not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_azureaduserfeatureusage"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.azureADUserFeatureUsage not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.azureADUserFeatureUsage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 748

{
  "value": {
    "@odata.type": "#microsoft.graph.azureADUserFeatureUsage",
    "id": "e64b9cd9-9cd9-e64b-d99c-4be6d99c4be6",
    "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00",
    "userId": "User Id value",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "licenseRecommended": "String",
    "licenseAssigned": "String",
    "featureUsageDetails": [
      {
        "@odata.type": "microsoft.graph.featureUsageDetail",
        "featureName": "Feature Name value",
        "licenseRequired": "String",
        "lastUsedDateTime": "2017-01-01T00:01:41.37493+03:00",
        "lastConfiguredDateTime": "2016-12-31T23:56:42.2289769+03:00"
      }
    ]
  }
}
```

