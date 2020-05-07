---
title: "Create shared"
description: "Create a new shared object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create shared

Namespace: microsoft.graph

Create a new shared object.

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
POST /users/{usersId}/insights/shared
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sharedInsight](../resources/sharedinsight.md) object.

The following table shows the properties that are required when you create the [sharedInsight](../resources/sharedinsight.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastShared|[sharingDetail](../resources/sharingdetail.md)|**TODO: Add Description**|
|sharingHistory|[sharingDetail](../resources/sharingdetail.md) collection|**TODO: Add Description**|
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)|**TODO: Add Description**|
|resourceReference|[resourceReference](../resources/resourcereference.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [sharedInsight](../resources/sharedinsight.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_sharedinsight_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/insights/shared
Content-Type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail"
  },
  "sharingHistory": [
    {
      "@odata.type": "microsoft.graph.sharingDetail"
    }
  ],
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedinsight"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "id": "dc3aeadc-eadc-dc3a-dcea-3adcdcea3adc",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail"
  },
  "sharingHistory": [
    {
      "@odata.type": "microsoft.graph.sharingDetail"
    }
  ],
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  }
}
```

