---
title: "List managedAppProtectionPolicySetItems"
description: "List properties and relationships of the managedAppProtectionPolicySetItem objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managedAppProtectionPolicySetItems

Namespace: microsoft.graph

List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md) objects.

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
GET ** Collection URI for microsoft.graph.managedAppProtectionPolicySetItem not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedAppProtectionPolicySetItem](../resources/managedappprotectionpolicysetitem.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedappprotectionpolicysetitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.managedAppProtectionPolicySetItem not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedappprotectionpolicysetitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
      "id": "491287de-87de-4912-de87-1249de871249",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "String",
      "errorCode": "String",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "targetedAppManagementLevels": "Targeted App Management Levels value"
    }
  ]
}
```

