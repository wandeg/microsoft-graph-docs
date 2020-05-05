---
title: "Update featureConfiguration"
description: "Update the properties of a featureConfiguration object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update featureConfiguration

Namespace: microsoft.cpim.api.dataModels

Update the properties of a [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object.

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
PATCH /identity/featureConfigurations/{featureConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object.

The following table shows the properties that are required when you create the [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|activatedFeatureTiers|identityFeatureTier|**TODO: Add Description**. Possible values are: `Standard`, `PremiumP1`, `PremiumP2`, `unknownFutureValue`.|
|azureResourceGroupName|String|**TODO: Add Description**|
|azureResourceName|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureSubscriptionTenantId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [featureConfiguration](../resources/microsoft.cpim.api.datamodels-featureconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_featureconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/featureConfigurations/{featureConfigurationId}
Content-Type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.cpim.api.dataModels.featureConfiguration",
  "activatedFeatureTiers": "String",
  "azureResourceGroupName": "Azure Resource Group Name value",
  "azureResourceName": "Azure Resource Name value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureSubscriptionTenantId": "Azure Subscription Tenant Id value"
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
{
  "@odata.type": "#microsoft.cpim.api.dataModels.featureConfiguration",
  "id": "ecfa2e2a-2e2a-ecfa-2a2e-faec2a2efaec",
  "activatedFeatureTiers": "String",
  "azureResourceGroupName": "Azure Resource Group Name value",
  "azureResourceName": "Azure Resource Name value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureSubscriptionTenantId": "Azure Subscription Tenant Id value"
}
```

