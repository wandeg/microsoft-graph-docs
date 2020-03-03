---
title: "Get emailAppUsageVersionsUserCounts"
description: "Read properties and relationships of the emailAppUsageVersionsUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get emailAppUsageVersionsUserCounts

Namespace: microsoft.graph

Read properties and relationships of the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.

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
GET ** Entity URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
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
If successful, this method returns a `200 OK` response code and [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailappusageversionsusercounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
    "id": "908104c9-04c9-9081-c904-8190c9048190",
    "reportRefreshDate": "Date",
    "outlook2016": 11,
    "outlook2013": 11,
    "outlook2010": 11,
    "outlook2007": 11,
    "undetermined": 12,
    "reportPeriod": "Report Period value"
  }
}
```

