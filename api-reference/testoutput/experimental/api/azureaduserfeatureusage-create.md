---
title: "Create azureADUserFeatureUsage"
description: "Create a new azureADUserFeatureUsage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create azureADUserFeatureUsage

Namespace: microsoft.graph

Create a new [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object.

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
POST ** Collection URI for microsoft.graph.azureADUserFeatureUsage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object.

The following table shows the properties that are required when you create the [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset||
|userId|String||
|userDisplayName|String||
|userPrincipalName|String||
|licenseRecommended|Enumeration|. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|licenseAssigned|Enumeration|. Possible values are: `none`, `free`, `basic`, `premiumP1`, `premiumP2`, `unknownFutureValue`.|
|featureUsageDetails|[featureUsageDetail](../resources/featureusagedetail.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_azureaduserfeatureusage_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.azureADUserFeatureUsage not found
Content-type: application/json
Content-length: 646

{
  "@odata.type": "#microsoft.graph.azureADUserFeatureUsage",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.azureaduserfeatureusage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
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
```

