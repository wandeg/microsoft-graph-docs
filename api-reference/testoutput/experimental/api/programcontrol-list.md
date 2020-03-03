---
title: "List programControls"
description: "List properties and relationships of the programControl objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List programControls

Namespace: microsoft.graph

List properties and relationships of the [programControl](../resources/programcontrol.md) objects.

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
GET /programControls
GET /programs/{programsId}/controls
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [programControl](../resources/programcontrol.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_programcontrol"
}
-->
``` http
GET https://graph.microsoft.com/localtest/programControls
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.programcontrol)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 745

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.programControl",
      "id": "59973866-3866-5997-6638-975966389759",
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
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00"
    }
  ]
}
```

