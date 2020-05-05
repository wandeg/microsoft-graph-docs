---
title: "Get featureConfiguration"
description: "Read properties and relationships of a featureConfiguration object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get featureConfiguration

Namespace: microsoft.cpim.api.dataModels

Read properties and relationships of a [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object.

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
GET /identity/featureConfigurations/{featureConfigurationId}
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
If successful, this method returns a `200 OK` response code and a [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_featureconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/featureConfigurations/{featureConfigurationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.dataModels.featureConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.cpim.api.dataModels.featureConfiguration",
    "id": "ecfa2e2a-2e2a-ecfa-2a2e-faec2a2efaec",
    "activatedFeatureTiers": "String",
    "azureResourceGroupName": "Azure Resource Group Name value",
    "azureResourceName": "Azure Resource Name value",
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureSubscriptionTenantId": "Azure Subscription Tenant Id value"
  }
}
```

