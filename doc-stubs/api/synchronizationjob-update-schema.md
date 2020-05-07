---
title: "Update schema"
description: "Update the properties of a schema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update schema

Namespace: microsoft.graph

Update the properties of a schema object.

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
PATCH /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [synchronizationSchema](../resources/synchronizationschema.md) object.

The following table shows the properties that are required when you create the [synchronizationSchema](../resources/synchronizationschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|provisioningTaskIdentifier|String|**TODO: Add Description**|
|synchronizationRules|[synchronizationRule](../resources/synchronizationrule.md) collection|**TODO: Add Description**|
|version|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [synchronizationSchema](../resources/synchronizationschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_schema"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema
Content-Type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "provisioningTaskIdentifier": "String",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "3ff23c40-3c40-3ff2-403c-f23f403cf23f",
  "provisioningTaskIdentifier": "String",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```

