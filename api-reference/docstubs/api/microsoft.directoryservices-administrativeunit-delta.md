---
title: "administrativeUnit: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# delta

Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

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
GET /administrativeUnits/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}
-->
``` http
GET https://graph.microsoft.com/changelog/administrativeUnits/delta
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.administrativeunit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.administrativeUnit",
      "id": "a2dd7382-7382-a2dd-8273-dda28273dda2",
      "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "visibility": "Visibility value"
    }
  ]
}
```

