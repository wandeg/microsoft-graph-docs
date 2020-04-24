---
title: "synchronizationSchema: filterOperators"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# filterOperators

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/filterOperators
GET /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema/filterOperators
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [filterOperatorSchema](../resources/filteroperatorschema.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/filterOperators
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.filteroperatorschema)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.filterOperatorSchema",
      "id": "505e5c17-5c17-505e-175c-5e50175c5e50",
      "arity": "String",
      "multivaluedComparisonType": "String",
      "supportedAttributeTypes": [
        "String"
      ]
    }
  ]
}
```

