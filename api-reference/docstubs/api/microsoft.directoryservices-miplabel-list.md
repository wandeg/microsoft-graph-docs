---
title: "List mipLabels"
description: "Get a list of the mipLabel objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List mipLabels

Namespace: Microsoft.DirectoryServices

Get a list of the [mipLabel](../resources/miplabel.md) objects and their properties.

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
GET /mipLabels
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
If successful, this method returns a `200 OK` response code and a collection of [mipLabel](../resources/miplabel.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_miplabel"
}
-->
``` http
GET https://graph.microsoft.com/changelog/mipLabels
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.miplabel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.mipLabel",
      "id": "042103df-03df-0421-df03-2104df032104",
      "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
      "labelId": "Label Id value",
      "displayName": "Display Name value",
      "protectGroupAction": {
        "@odata.type": "Microsoft.DirectoryServices.mipProtectGroupLabelAction",
        "isAccessAllowedToGuestUsers": true,
        "privacy": "Privacy value"
      }
    }
  ]
}
```

