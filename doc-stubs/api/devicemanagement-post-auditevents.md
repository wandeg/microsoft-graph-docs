---
title: "Create auditEvents"
description: "Create a new auditEvents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create auditEvents

Namespace: microsoft.graph

Create a new auditEvents object.

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
POST /deviceManagement/auditEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [auditEvent](../resources/auditevent.md) object.

The following table shows the properties that are required when you create the [auditEvent](../resources/auditevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|componentName|String|**TODO: Add Description**|
|actor|[auditActor](../resources/auditactor.md)|**TODO: Add Description**|
|activity|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|activityType|String|**TODO: Add Description**|
|activityOperationType|String|**TODO: Add Description**|
|activityResult|String|**TODO: Add Description**|
|correlationId|Guid|**TODO: Add Description**|
|resources|[auditResource](../resources/auditresource.md) collection|**TODO: Add Description**|
|category|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [auditEvent](../resources/auditevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_auditevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-Type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource"
    }
  ],
  "category": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "a4e59548-9548-a4e5-4895-e5a44895e5a4",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource"
    }
  ],
  "category": "String"
}
```

