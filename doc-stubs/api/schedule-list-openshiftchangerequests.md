---
title: "List openShiftChangeRequests"
description: "Get the openShiftChangeRequests from the openShiftChangeRequests navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List openShiftChangeRequests

Namespace: microsoft.graph

Get the openShiftChangeRequests from the openShiftChangeRequests navigation property.

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
GET /teams/{teamsId}/schedule/openShiftChangeRequests
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/{teamsId}/schedule/openShiftChangeRequests
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.openshiftchangerequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.openShiftChangeRequest",
      "id": "16fb7157-7157-16fb-5771-fb165771fb16",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "assignedTo": "String",
      "state": "String",
      "senderMessage": "String",
      "senderDateTime": "String (timestamp)",
      "managerActionMessage": "String",
      "managerActionDateTime": "String (timestamp)",
      "senderUserId": "String",
      "managerUserId": "String",
      "openShiftId": "String"
    }
  ]
}
```

