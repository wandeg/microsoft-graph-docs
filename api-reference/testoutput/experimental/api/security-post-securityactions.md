---
title: "Add securityActions"
description: "Add securityActions by posting to the securityActions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add securityActions

Namespace: microsoft.graph

Add securityActions by posting to the securityActions collection.

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
POST /Security/securityActions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [securityAction](../resources/securityaction.md) object.

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
|errorInfo|[ResultInfo](../resources/resultinfo.md)||
|lastActionDateTime|DateTimeOffset||
|name|String||
|parameters|[keyValuePair](../resources/keyvaluepair.md) collection||
|states|[securityActionState](../resources/securityactionstate.md) collection||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/Security/securityActions
Content-type: application/json
Content-length: 1143

{
  "@odata.type": "#microsoft.graph.securityAction",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:01:22.3370207+03:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00",
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
      "updatedDateTime": "2016-12-31T23:56:50.0206912+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.securityaction"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1250

{
  "@odata.type": "#microsoft.graph.securityAction",
  "id": "88effc58-fc58-88ef-58fc-ef8858fcef88",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:01:22.3370207+03:00",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00",
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
      "updatedDateTime": "2016-12-31T23:56:50.0206912+03:00",
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

