---
title: "List programControls"
description: "Get a list of the programControl objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
GET https://graph.microsoft.com/beta/programControls
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
      "id": "f522c821-c821-f522-21c8-22f521c822f5",
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
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00"
    }
  ]
}
```

