---
title: "List mailboxUsageStorages"
description: "List properties and relationships of the mailboxUsageStorage objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mailboxUsageStorages

List properties and relationships of the [mailboxUsageStorage](../resources/mailboxusagestorage.md) objects.

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
GET ** Collection URI for microsoft.graph.mailboxUsageStorage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mailboxUsageStorage](../resources/mailboxusagestorage.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailboxusagestorage"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.mailboxUsageStorage not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailboxusagestorage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailboxUsageStorage",
      "id": "d975738f-738f-d975-8f73-75d98f7375d9",
      "reportRefreshDate": "Date",
      "storageUsedInBytes": 2,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

