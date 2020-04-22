---
title: "List domains"
description: "Get a list of the domain objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List domains

Namespace: microsoft.graph

Get a list of the [domain](../resources/domain.md) objects and their properties.

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
GET /domains
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [domain](../resources/domain.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domain"
}
-->
``` http
GET https://graph.microsoft.com/beta/domains
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domain)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domain",
      "id": "73f8a0d7-a0d7-73f8-d7a0-f873d7a0f873",
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
        "lastActionDateTime": "2017-01-01T00:01:03.6946751+00:00"
      }
    }
  ]
}
```

