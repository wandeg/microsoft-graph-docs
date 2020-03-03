---
title: "List definitionValues"
description: "Get the groupPolicyDefinitionValues from the definitionValues navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List definitionValues

Get the groupPolicyDefinitionValues from the definitionValues navigation property.

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
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicydefinitionvalue"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
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
Content-Length: 351

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "id": "b16ccc23-cc23-b16c-23cc-6cb123cc6cb1",
      "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
      "enabled": true,
      "configurationType": "String",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
    }
  ]
}
```

