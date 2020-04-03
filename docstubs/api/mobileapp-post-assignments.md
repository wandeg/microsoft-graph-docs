---
title: "Add assignments"
description: "Add assignments by posting to the assignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add assignments

Namespace: microsoft.graph

Add assignments by posting to the assignments collection.

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/mobileappassignment.md) object.

The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/mobileappassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|intent|Enumeration| Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||
|settings|[mobileAppAssignmentSettings](../resources/mobileappassignmentsettings.md)||
|source|Enumeration| Possible values are: `direct`, `policySets`.|
|sourceId|String||



## Response
If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/mobileappassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileappassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 328

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "String",
  "sourceId": "Source Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileappassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "e1974891-4891-e197-9148-97e1914897e1",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "String",
  "sourceId": "Source Id value"
}
```

