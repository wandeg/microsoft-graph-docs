---
title: "List groupPolicyMigrationReports"
description: "Get the groupPolicyMigrationReports from the groupPolicyMigrationReports navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicyMigrationReports

Namespace: microsoft.graph

Get the groupPolicyMigrationReports from the groupPolicyMigrationReports navigation property.

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
GET /deviceManagement/groupPolicyMigrationReports
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
If successful, this method returns a `200 OK` response code and a collection of [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicymigrationreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicymigrationreport)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 804

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
      "id": "538fd1be-d1be-538f-bed1-8f53bed18f53",
      "groupPolicyObjectId": "c500b80c-b80c-c500-0cb8-00c50cb800c5",
      "displayName": "Display Name value",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
      "groupPolicyCreatedDateTime": "2017-01-01T00:02:06.1917427+00:00",
      "groupPolicyLastModifiedDateTime": "2017-01-01T00:00:26.9843205+00:00",
      "migrationReadiness": "String",
      "targetedInActiveDirectory": true,
      "totalSettingsCount": 2,
      "supportedSettingsCount": 6,
      "supportedSettingsPercent": 8
    }
  ]
}
```

