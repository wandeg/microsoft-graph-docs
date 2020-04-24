---
title: "Create securityActions"
description: "Create a new securityActions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create securityActions

Namespace: microsoft.graph

Create a new securityActions object.

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
POST /Security/securityActions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [securityAction](../resources/securityaction.md) object.

The following table shows the properties that are required when you create the [securityAction](../resources/securityaction.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|actionReason|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|clientContext|String|**TODO: Add Description**|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|errorInfo|[ResultInfo](../resources/resultinfo.md)|**TODO: Add Description**|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|parameters|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|states|[securityActionState](../resources/securityactionstate.md) collection|**TODO: Add Description**|
|status|operationStatus|**TODO: Add Description**. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/securityActions
Content-Type: application/json
Content-length: 1142

{
  "@odata.type": "#microsoft.graph.securityAction",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:02:03.9770517+03:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:57:13.8078619+03:00",
  "name": "Name value",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "value": "Value value"
    }
  ],
  "states": [
    {
      "@odata.type": "microsoft.graph.securityActionState",
      "status": "String",
      "updatedDateTime": "2017-01-01T00:00:22.114869+03:00",
      "user": "User value"
    }
  ],
  "status": "String",
  "user": "User value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityaction"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.securityAction",
  "id": "cf3a5d69-5d69-cf3a-695d-3acf695d3acf",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:02:03.9770517+03:00",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:57:13.8078619+03:00",
  "name": "Name value",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "value": "Value value"
    }
  ],
  "states": [
    {
      "@odata.type": "microsoft.graph.securityActionState",
      "status": "String",
      "updatedDateTime": "2017-01-01T00:00:22.114869+03:00",
      "user": "User value"
    }
  ],
  "status": "String",
  "user": "User value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

