---
title: "List definitionValues"
description: "Get the groupPolicyDefinitionValues from the definitionValues navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List definitionValues

Namespace: microsoft.graph

Get the groupPolicyDefinitionValues from the definitionValues navigation property.

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
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
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
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicydefinitionvalue"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicydefinitionvalue)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 350

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "id": "bb19a523-a523-bb19-23a5-19bb23a519bb",
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
      "enabled": true,
      "configurationType": "String",
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00"
    }
  ]
}
```

