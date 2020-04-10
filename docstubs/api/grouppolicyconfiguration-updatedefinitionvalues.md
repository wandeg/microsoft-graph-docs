---
title: "groupPolicyConfiguration: updateDefinitionValues"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# updateDefinitionValues

Namespace: microsoft.graph



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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|added|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection||
|updated|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection||
|deletedIds|String collection||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "grouppolicyconfiguration_updatedefinitionvalues"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues

Content-type: application/json
Content-length: 751

{
  "added": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "id": "4a497b69-7b69-4a49-697b-494a697b494a",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "enabled": true,
      "configurationType": "String",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
    }
  ],
  "updated": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "id": "4a497b69-7b69-4a49-697b-494a697b494a",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "enabled": true,
      "configurationType": "String",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
    }
  ],
  "deletedIds": [
    "Deleted Ids value"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

