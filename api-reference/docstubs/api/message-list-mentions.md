---
title: "List mentions"
description: "Get the mentions from the mentions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mentions

Namespace: microsoft.graph

Get the mentions from the mentions navigation property.

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
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/mentions
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
If successful, this method returns a `200 OK` response code and a collection of [mention](../resources/mention.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mention"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/messages/{messageId}/mentions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mention)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mention",
      "id": "1bee794f-794f-1bee-4f79-ee1b4f79ee1b",
      "mentioned": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      },
      "mentionText": "Mention Text value",
      "clientReference": "Client Reference value",
      "createdBy": {
        "@odata.type": "microsoft.graph.emailAddress"
      },
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "serverCreatedDateTime": "2017-01-01T00:02:35.5937708+03:00",
      "deepLink": "Deep Link value",
      "application": "Application value"
    }
  ]
}
```

