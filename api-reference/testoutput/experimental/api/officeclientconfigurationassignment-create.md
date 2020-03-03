---
title: "Create officeClientConfigurationAssignment"
description: "Create a new officeClientConfigurationAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create officeClientConfigurationAssignment

Namespace: microsoft.graph

Create a new [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object.

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
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object.

The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[officeConfigurationAssignmentTarget](../resources/officeconfigurationassignmenttarget.md)||



## Response
If successful, this method returns a `201 Created` response code and a [officeClientConfigurationAssignment](../resources/officeclientconfigurationassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_officeclientconfigurationassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officeclientconfigurationassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "08f87e97-7e97-08f8-977e-f808977ef808",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

