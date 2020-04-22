---
title: "List programControls"
description: "Get a list of the programControl objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List programControls

Namespace: microsoft.graph

Get a list of the [programControl](../resources/programcontrol.md) objects and their properties.

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
GET /programControls
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
If successful, this method returns a `200 OK` response code and a collection of [programControl](../resources/programcontrol.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_programcontrol"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/programControls
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.programcontrol)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.programControl",
      "id": "5a1d1496-1496-5a1d-9614-1d5a96141d5a",
      "controlId": "Control Id value",
      "programId": "Program Id value",
      "controlTypeId": "Control Type Id value",
      "displayName": "Display Name value",
      "status": "Status value",
      "owner": {
        "@odata.type": "microsoft.graph.userIdentity",
        "id": "Id value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      },
      "resource": {
        "@odata.type": "microsoft.graph.programResource",
        "type": "Type value"
      },
      "createdDateTime": "2017-01-01T00:02:14.13292+00:00"
    }
  ]
}
```

