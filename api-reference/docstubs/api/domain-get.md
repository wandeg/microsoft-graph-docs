---
title: "Get domain"
description: "Read the properties and relationships of a domain object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get domain

Namespace: microsoft.graph

Read the properties and relationships of a [domain](../resources/domain.md) object.

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
GET /domains/{domainsId}
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
If successful, this method returns a `200 OK` response code and a [domain](../resources/domain.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domain"
}
-->
``` http
GET https://graph.microsoft.com/beta/domains/{domainsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.domain",
    "id": "a2294f8a-4f8a-a229-8a4f-29a28a4f29a2",
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
      "lastActionDateTime": "2017-01-01T00:02:49.8376032+03:00"
    }
  }
}
```

