---
title: "Get groupPolicyPresentationListBox"
description: "Read properties and relationships of the groupPolicyPresentationListBox object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupPolicyPresentationListBox

Namespace: microsoft.graph

Read properties and relationships of the [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md) object.

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
GET ** Entity URI for microsoft.graph.groupPolicyPresentationListBox not found
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
If successful, this method returns a `200 OK` response code and [groupPolicyPresentationListBox](../resources/grouppolicypresentationlistbox.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicypresentationlistbox"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.groupPolicyPresentationListBox not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
    "id": "bc4e845d-845d-bc4e-5d84-4ebc5d844ebc",
    "label": "Label value",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
    "explicitValue": true,
    "valuePrefix": "Value Prefix value"
  }
}
```

