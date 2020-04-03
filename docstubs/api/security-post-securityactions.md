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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /Security/securityActions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
|status|Enumeration| Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/securityActions
Content-type: application/json
Content-length: 1142

{
  "@odata.type": "#microsoft.graph.securityAction",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:03:18.4386811+00:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:58:25.2668755+00:00",
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
      "updatedDateTime": "2017-01-01T00:02:17.171024+00:00",
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
  "id": "6934a43d-a43d-6934-3da4-34693da43469",
  "actionReason": "Action Reason value",
  "appId": "App Id value",
  "azureTenantId": "Azure Tenant Id value",
  "clientContext": "Client Context value",
  "completedDateTime": "2017-01-01T00:03:18.4386811+00:00",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "errorInfo": {
    "@odata.type": "microsoft.graph.ResultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "lastActionDateTime": "2016-12-31T23:58:25.2668755+00:00",
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
      "updatedDateTime": "2017-01-01T00:02:17.171024+00:00",
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

