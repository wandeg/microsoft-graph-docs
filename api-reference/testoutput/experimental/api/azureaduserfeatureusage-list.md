---
title: "List azureADUserFeatureUsages"
description: "List properties and relationships of the azureADUserFeatureUsage objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List azureADUserFeatureUsages

List properties and relationships of the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) objects.

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
GET ** Collection URI for microsoft.graph.azureADUserFeatureUsage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_azureaduserfeatureusage"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.azureADUserFeatureUsage not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.azureaduserfeatureusage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 798

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.azureADUserFeatureUsage",
      "id": "661c46de-46de-661c-de46-1c66de461c66",
      "lastUpdatedDateTime": "2017-01-01T00:01:04.1563754+03:00",
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
          "lastUsedDateTime": "2016-12-31T23:57:25.2787332+03:00",
          "lastConfiguredDateTime": "2016-12-31T23:58:54.8342461+03:00"
        }
      ]
    }
  ]
}
```

