---
title: "List threatAssessmentRequests"
description: "Get the threatAssessmentRequests from the threatAssessmentRequests navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List threatAssessmentRequests

Namespace: microsoft.graph

Get the threatAssessmentRequests from the threatAssessmentRequests navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/threatAssessmentRequests
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.threatassessmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 803

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.threatAssessmentRequest",
      "id": "f1dcfab8-fab8-f1dc-b8fa-dcf1b8fadcf1",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "contentType": "String",
      "expectedAssessment": "String",
      "category": "String",
      "status": "String",
      "requestSource": "String",
      "createdBy": {
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
      }
    }
  ]
}
```

