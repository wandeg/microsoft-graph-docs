---
title: "Get targetedManagedAppConfigurationPolicySetItem"
description: "Read properties and relationships of the targetedManagedAppConfigurationPolicySetItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get targetedManagedAppConfigurationPolicySetItem

Namespace: microsoft.graph

Read properties and relationships of the [targetedManagedAppConfigurationPolicySetItem](../resources/targetedmanagedappconfigurationpolicysetitem.md) object.

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
GET ** Entity URI for microsoft.graph.targetedManagedAppConfigurationPolicySetItem not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [targetedManagedAppConfigurationPolicySetItem](../resources/targetedmanagedappconfigurationpolicysetitem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_targetedmanagedappconfigurationpolicysetitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.targetedManagedAppConfigurationPolicySetItem not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.targetedManagedAppConfigurationPolicySetItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 530

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
    "id": "b227d584-d584-b227-84d5-27b284d527b2",
    "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "String",
    "errorCode": "String",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ]
  }
}
```

