---
title: "Get scheduleChangeRequest"
description: "Read properties and relationships of the scheduleChangeRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get scheduleChangeRequest

Namespace: microsoft.graph

Read properties and relationships of the [scheduleChangeRequest](../resources/schedulechangerequest.md) object.

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
GET ** Entity URI for microsoft.graph.scheduleChangeRequest not found
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
If successful, this method returns a `200 OK` response code and [scheduleChangeRequest](../resources/schedulechangerequest.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schedulechangerequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.scheduleChangeRequest not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleChangeRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1041

{
  "value": {
    "@odata.type": "#microsoft.graph.scheduleChangeRequest",
    "id": "1b4ee48a-e48a-1b4e-8ae4-4e1b8ae44e1b",
    "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "assignedTo": "String",
    "state": "String",
    "senderMessage": "Sender Message value",
    "senderDateTime": "2016-12-31T23:59:47.8447466+03:00",
    "managerActionMessage": "Manager Action Message value",
    "managerActionDateTime": "2017-01-01T00:03:26.1696907+03:00",
    "senderUserId": "Sender User Id value",
    "managerUserId": "Manager User Id value"
  }
}
```

