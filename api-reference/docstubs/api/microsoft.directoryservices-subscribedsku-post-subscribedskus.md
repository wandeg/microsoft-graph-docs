---
title: "Create subscribedSku"
description: "Create a new subscribedSku object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create subscribedSku

Namespace: Microsoft.DirectoryServices

Create a new [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) object.

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
POST /subscribedSkus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) object.

The following table shows the properties that are required when you create the [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md).

|Property|Type|Description|
|:---|:---|:---|
|capabilityStatus|String|**TODO: Add Description**|
|consumedUnits|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|prepaidUnits|[licenseUnitsDetail](../resources/microsoft.directoryservices-licenseunitsdetail.md)|**TODO: Add Description**|
|servicePlans|[servicePlanInfo](../resources/microsoft.directoryservices-serviceplaninfo.md) collection|**TODO: Add Description**|
|skuId|Guid|**TODO: Add Description**|
|skuPartNumber|String|**TODO: Add Description**|
|appliesTo|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [subscribedSku](../resources/microsoft.directoryservices-subscribedsku.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_subscribedsku_from_subscribedskus"
}
-->
``` http
POST https://graph.microsoft.com/changelog/subscribedSkus
Content-Type: application/json
Content-length: 753

{
  "@odata.type": "#Microsoft.DirectoryServices.subscribedSku",
  "capabilityStatus": "Capability Status value",
  "consumedUnits": 13,
  "prepaidUnits": {
    "@odata.type": "Microsoft.DirectoryServices.licenseUnitsDetail",
    "enabled": 7,
    "suspended": 9,
    "warning": 7
  },
  "servicePlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.servicePlanInfo",
      "servicePlanId": "4545cb79-cb79-4545-79cb-454579cb4545",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "92ad2f35-2f35-92ad-352f-ad92352fad92",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.subscribedsku"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.subscribedSku",
  "capabilityStatus": "Capability Status value",
  "consumedUnits": 13,
  "id": "24d657de-57de-24d6-de57-d624de57d624",
  "prepaidUnits": {
    "@odata.type": "Microsoft.DirectoryServices.licenseUnitsDetail",
    "enabled": 7,
    "suspended": 9,
    "warning": 7
  },
  "servicePlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.servicePlanInfo",
      "servicePlanId": "4545cb79-cb79-4545-79cb-454579cb4545",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "92ad2f35-2f35-92ad-352f-ad92352fad92",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
}
```

