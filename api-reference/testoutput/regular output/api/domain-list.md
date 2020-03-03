---
title: "List domains"
description: "List properties and relationships of the domain objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List domains

Namespace: microsoft.graph

List properties and relationships of the [domain](../resources/domain.md) objects.

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
GET /domains
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [domain](../resources/domain.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domain"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domains
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domain)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domain",
      "id": "47a61309-1309-47a6-0913-a6470913a647",
      "authenticationType": "Authentication Type value",
      "availabilityStatus": "Availability Status value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "isVerified": true,
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "passwordNotificationWindowInDays": 0,
      "passwordValidityPeriodInDays": 12,
      "supportedServices": [
        "Supported Services value"
      ],
      "state": {
        "@odata.type": "microsoft.graph.domainState",
        "status": "Status value",
        "operation": "Operation value",
        "lastActionDateTime": "2017-01-01T00:02:27.6832592+03:00"
      }
    }
  ]
}
```

