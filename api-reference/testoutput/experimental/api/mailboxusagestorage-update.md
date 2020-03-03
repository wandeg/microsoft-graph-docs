---
title: "Update mailboxUsageStorage"
description: "Update the properties of a mailboxUsageStorage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mailboxUsageStorage

Update the properties of a [mailboxUsageStorage](../resources/mailboxusagestorage.md) object.

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
PATCH ** Entity URI for microsoft.graph.mailboxUsageStorage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [mailboxUsageStorage](../resources/mailboxUsageStorage.md) object.

The following table shows the properties that are required when you create the [mailboxUsageStorage](../resources/mailboxusagestorage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|storageUsedInBytes|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [mailboxUsageStorage](../resources/mailboxusagestorage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mailboxusagestorage"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.mailboxUsageStorage not found
Content-type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.mailboxUsageStorage",
  "reportRefreshDate": "Date",
  "storageUsedInBytes": 2,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.mailboxUsageStorage",
  "id": "d975738f-738f-d975-8f73-75d98f7375d9",
  "reportRefreshDate": "Date",
  "storageUsedInBytes": 2,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

