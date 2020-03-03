---
title: "List termsAndConditionsAcceptanceStatuses"
description: "List properties and relationships of the termsAndConditionsAcceptanceStatus objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List termsAndConditionsAcceptanceStatuses

Namespace: microsoft.graph

List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) objects.

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
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_termsandconditionsacceptancestatus"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termsandconditionsacceptancestatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "1f5f4d2e-4d2e-1f5f-2e4d-5f1f2e4d5f1f",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2017-01-01T00:00:56.6153418+03:00"
    }
  ]
}
```

