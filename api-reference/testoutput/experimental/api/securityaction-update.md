---
title: "Update securityAction"
description: "Update the properties of a securityAction object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update securityAction

Update the properties of a [securityAction](../resources/securityaction.md) object.

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
PATCH /Security/securityActions/{securityActionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [securityAction](../resources/securityAction.md) object.

The following table shows the properties that are required when you create the [securityAction](../resources/securityaction.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|actionReason|String||
|appId|String||
|azureTenantId|String||
|clientContext|String||
|completedDateTime|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|errorInfo|[ResultInfo](../resources/ResultInfo.md)||
|lastActionDateTime|DateTimeOffset||
|name|String||
|parameters|[keyValuePair](../resources/keyValuePair.md) collection||
|states|[securityActionState](../resources/securityActionState.md) collection||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String||
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [securityAction](../resources/securityaction.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_securityaction"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/Security/securityActions/{securityActionId}
Content-type: application/json
Content-length: 1143

{
  "@odata.type": "#microsoft.graph.securityAction",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:01:13.9669573+03:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:56:44.8542569+03:00",
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
      "updatedDateTime": "2017-01-01T00:02:44.8627183+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.securityAction",
  "id": "eb659326-9326-eb65-2693-65eb269365eb",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:01:13.9669573+03:00",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:56:44.8542569+03:00",
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
      "updatedDateTime": "2017-01-01T00:02:44.8627183+03:00",
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

