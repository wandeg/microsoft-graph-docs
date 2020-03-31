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
Content-Length: 803

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
      "id": "ab973e2f-3e2f-ab97-2f3e-97ab2f3e97ab",
      "groupPolicyObjectId": "78ef7982-7982-78ef-8279-ef788279ef78",
      "displayName": "Display Name value",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
      "groupPolicyCreatedDateTime": "2016-12-31T23:57:29.4861742+03:00",
      "groupPolicyLastModifiedDateTime": "2017-01-01T00:00:03.0868943+03:00",
      "migrationReadiness": "String",
      "targetedInActiveDirectory": true,
      "totalSettingsCount": 2,
      "supportedSettingsCount": 6,
      "supportedSettingsPercent": 8
    }
  ]
}
```

