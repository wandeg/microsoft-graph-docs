---
title: "List resources"
description: "Get the educationAssignmentResources from the resources navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List resources

Namespace: microsoft.graph

Get the educationAssignmentResources from the resources navigation property.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources
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
If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationassignmentresource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationAssignmentResource",
      "id": "c4afcce4-cce4-c4af-e4cc-afc4e4ccafc4",
      "distributeForStudentWork": true,
      "resource": {
        "@odata.type": "microsoft.graph.educationResource",
        "displayName": "Display Name value",
        "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
        "createdBy": {
          "@odata.type": "microsoft.graph.identitySet",
          "application": {
            "@odata.type": "microsoft.graph.identity",
            "id": "Id value"
          },
          "device": {
            "@odata.type": "microsoft.graph.identity"
          },
          "user": {
            "@odata.type": "microsoft.graph.identity"
          }
        },
        "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
        "lastModifiedBy": {
          "@odata.type": "microsoft.graph.identitySet"
        }
      }
    }
  ]
}
```

