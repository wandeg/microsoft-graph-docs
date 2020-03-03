---
title: "Get domain"
description: "Read properties and relationships of the domain object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get domain

Namespace: microsoft.graph

Read properties and relationships of the [domain](../resources/domain.md) object.

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
GET /domains/{domainsId}
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
If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domain"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domains/{domainsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 724

{
  "value": {
    "@odata.type": "#microsoft.graph.domain",
    "id": "91491c9e-1c9e-9149-9e1c-49919e1c4991",
    "authenticationType": "Authentication Type value",
    "availabilityStatus": "Availability Status value",
    "isAdminManaged": true,
    "isDefault": true,
    "isInitial": true,
    "isRoot": true,
    "isVerified": true,
    "passwordNotificationWindowInDays": 0,
    "passwordValidityPeriodInDays": 12,
    "supportedServices": [
      "Supported Services value"
    ],
    "state": {
      "@odata.type": "microsoft.graph.domainState",
      "status": "Status value",
      "operation": "Operation value",
      "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00"
    }
  }
}
```

