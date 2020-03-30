---
title: "Get managedAppPolicyDeploymentSummary"
description: "Read properties and relationships of the managedAppPolicyDeploymentSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get managedAppPolicyDeploymentSummary

Namespace: microsoft.graph

Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.

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
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedapppolicydeploymentsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "id": "f616be38-be38-f616-38be-16f638be16f6",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:03:12.4957446+03:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "version": "Version value"
  }
}
```

