---
title: "Update alert"
description: "Update the properties of a alert object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update alert

Namespace: microsoft.graph

Update the properties of a [alert](../resources/alert.md) object.

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
PATCH /Security/alerts/{alertId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [alert](../resources/alert.md) object.

The following table shows the properties that are required when you create the [alert](../resources/alert.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activityGroupName|String|**TODO: Add Description**|
|assignedTo|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|category|String|**TODO: Add Description**|
|closedDateTime|DateTimeOffset|**TODO: Add Description**|
|cloudAppStates|[cloudAppSecurityState](../resources/cloudappsecuritystate.md) collection|**TODO: Add Description**|
|comments|String collection|**TODO: Add Description**|
|confidence|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|detectionIds|String collection|**TODO: Add Description**|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|
|feedback|alertFeedback|**TODO: Add Description**. Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`, `unknownFutureValue`.|
|fileStates|[fileSecurityState](../resources/filesecuritystate.md) collection|**TODO: Add Description**|
|historyStates|[alertHistoryState](../resources/alerthistorystate.md) collection|**TODO: Add Description**|
|hostStates|[hostSecurityState](../resources/hostsecuritystate.md) collection|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareStates|[malwareState](../resources/malwarestate.md) collection|**TODO: Add Description**|
|networkConnections|[networkConnection](../resources/networkconnection.md) collection|**TODO: Add Description**|
|processes|[process](../resources/process.md) collection|**TODO: Add Description**|
|recommendedActions|String collection|**TODO: Add Description**|
|registryKeyStates|[registryKeyState](../resources/registrykeystate.md) collection|**TODO: Add Description**|
|severity|alertSeverity|**TODO: Add Description**. Possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`.|
|sourceMaterials|String collection|**TODO: Add Description**|
|status|alertStatus|**TODO: Add Description**. Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`, `unknownFutureValue`.|
|tags|String collection|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|triggers|[alertTrigger](../resources/alerttrigger.md) collection|**TODO: Add Description**|
|userStates|[userSecurityState](../resources/usersecuritystate.md) collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [alert](../resources/alert.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_alert"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/alerts/{alertId}
Content-Type: application/json
Content-length: 5208

{
  "@odata.type": "#microsoft.graph.alert",
  "activityGroupName": "Activity Group Name value",
  "assignedTo": "Assigned To value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "category": "Category value",
  "closedDateTime": "2016-12-31T23:57:14.8031051+00:00",
  "cloudAppStates": [
    {
      "@odata.type": "microsoft.graph.cloudAppSecurityState",
      "destinationServiceIp": "Destination Service Ip value",
      "destinationServiceName": "Destination Service Name value",
      "riskScore": "Risk Score value"
    }
  ],
  "comments": [
    "Comments value"
  ],
  "confidence": 10,
  "description": "Description value",
  "detectionIds": [
    "Detection Ids value"
  ],
  "eventDateTime": "2016-12-31T23:57:29.5616003+00:00",
  "feedback": "String",
  "fileStates": [
    {
      "@odata.type": "microsoft.graph.fileSecurityState",
      "fileHash": {
        "@odata.type": "microsoft.graph.fileHash",
        "hashType": "String",
        "hashValue": "Hash Value value"
      },
      "name": "Name value",
      "path": "Path value"
    }
  ],
  "historyStates": [
    {
      "@odata.type": "microsoft.graph.alertHistoryState",
      "appId": "App Id value",
      "status": "String",
      "updatedDateTime": "2016-12-31T23:58:27.5767592+00:00",
      "user": "User value"
    }
  ],
  "hostStates": [
    {
      "@odata.type": "microsoft.graph.hostSecurityState",
      "fqdn": "Fqdn value",
      "isAzureAdJoined": true,
      "isAzureAdRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "Net Bios Name value",
      "os": "Os value",
      "privateIpAddress": "Private Ip Address value",
      "publicIpAddress": "Public Ip Address value"
    }
  ],
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState",
      "family": "Family value",
      "severity": "Severity value",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "@odata.type": "microsoft.graph.networkConnection",
      "applicationName": "Application Name value",
      "destinationAddress": "Destination Address value",
      "destinationDomain": "Destination Domain value",
      "destinationPort": "Destination Port value",
      "destinationUrl": "https://example.com/destinationUrl/",
      "direction": "String",
      "domainRegisteredDateTime": "2016-12-31T23:58:42.9000822+00:00",
      "localDnsName": "Local Dns Name value",
      "natDestinationAddress": "Nat Destination Address value",
      "natDestinationPort": "Nat Destination Port value",
      "natSourceAddress": "Nat Source Address value",
      "natSourcePort": "Nat Source Port value",
      "protocol": "String",
      "sourceAddress": "Source Address value",
      "sourcePort": "Source Port value",
      "status": "String",
      "urlParameters": "Url Parameters value"
    }
  ],
  "processes": [
    {
      "@odata.type": "microsoft.graph.process",
      "accountName": "Account Name value",
      "commandLine": "Command Line value",
      "integrityLevel": "String",
      "isElevated": true,
      "parentProcessCreatedDateTime": "2016-12-31T23:59:05.910252+00:00",
      "parentProcessId": 15,
      "parentProcessName": "Parent Process Name value",
      "processId": 9
    }
  ],
  "recommendedActions": [
    "Recommended Actions value"
  ],
  "registryKeyStates": [
    {
      "@odata.type": "microsoft.graph.registryKeyState",
      "hive": "String",
      "key": "Key value",
      "oldKey": "Old Key value",
      "oldValueData": "Old Value Data value",
      "oldValueName": "Old Value Name value",
      "operation": "String",
      "valueData": "Value Data value",
      "valueName": "Value Name value",
      "valueType": "String"
    }
  ],
  "severity": "String",
  "sourceMaterials": [
    "Source Materials value"
  ],
  "status": "String",
  "tags": [
    "Tags value"
  ],
  "title": "Title value",
  "triggers": [
    {
      "@odata.type": "microsoft.graph.alertTrigger",
      "type": "Type value",
      "value": "Value value"
    }
  ],
  "userStates": [
    {
      "@odata.type": "microsoft.graph.userSecurityState",
      "aadUserId": "Aad User Id value",
      "domainName": "Domain Name value",
      "emailRole": "String",
      "isVpn": true,
      "logonDateTime": "2016-12-31T23:57:12.5063859+00:00",
      "logonId": "Logon Id value",
      "logonIp": "Logon Ip value",
      "logonLocation": "Logon Location value",
      "logonType": "String",
      "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
      "userAccountType": "String",
      "userPrincipalName": "User Principal Name value"
    }
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState",
      "cve": "Cve value"
    }
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
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.alert",
  "id": "c5a19d36-9d36-c5a1-369d-a1c5369da1c5",
  "activityGroupName": "Activity Group Name value",
  "assignedTo": "Assigned To value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "category": "Category value",
  "closedDateTime": "2016-12-31T23:57:14.8031051+00:00",
  "cloudAppStates": [
    {
      "@odata.type": "microsoft.graph.cloudAppSecurityState",
      "destinationServiceIp": "Destination Service Ip value",
      "destinationServiceName": "Destination Service Name value",
      "riskScore": "Risk Score value"
    }
  ],
  "comments": [
    "Comments value"
  ],
  "confidence": 10,
  "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
  "description": "Description value",
  "detectionIds": [
    "Detection Ids value"
  ],
  "eventDateTime": "2016-12-31T23:57:29.5616003+00:00",
  "feedback": "String",
  "fileStates": [
    {
      "@odata.type": "microsoft.graph.fileSecurityState",
      "fileHash": {
        "@odata.type": "microsoft.graph.fileHash",
        "hashType": "String",
        "hashValue": "Hash Value value"
      },
      "name": "Name value",
      "path": "Path value"
    }
  ],
  "historyStates": [
    {
      "@odata.type": "microsoft.graph.alertHistoryState",
      "appId": "App Id value",
      "status": "String",
      "updatedDateTime": "2016-12-31T23:58:27.5767592+00:00",
      "user": "User value"
    }
  ],
  "hostStates": [
    {
      "@odata.type": "microsoft.graph.hostSecurityState",
      "fqdn": "Fqdn value",
      "isAzureAdJoined": true,
      "isAzureAdRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "Net Bios Name value",
      "os": "Os value",
      "privateIpAddress": "Private Ip Address value",
      "publicIpAddress": "Public Ip Address value"
    }
  ],
  "lastModifiedDateTime": "2017-01-01T00:01:26.0388723+00:00",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState",
      "family": "Family value",
      "severity": "Severity value",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "@odata.type": "microsoft.graph.networkConnection",
      "applicationName": "Application Name value",
      "destinationAddress": "Destination Address value",
      "destinationDomain": "Destination Domain value",
      "destinationPort": "Destination Port value",
      "destinationUrl": "https://example.com/destinationUrl/",
      "direction": "String",
      "domainRegisteredDateTime": "2016-12-31T23:58:42.9000822+00:00",
      "localDnsName": "Local Dns Name value",
      "natDestinationAddress": "Nat Destination Address value",
      "natDestinationPort": "Nat Destination Port value",
      "natSourceAddress": "Nat Source Address value",
      "natSourcePort": "Nat Source Port value",
      "protocol": "String",
      "sourceAddress": "Source Address value",
      "sourcePort": "Source Port value",
      "status": "String",
      "urlParameters": "Url Parameters value"
    }
  ],
  "processes": [
    {
      "@odata.type": "microsoft.graph.process",
      "accountName": "Account Name value",
      "commandLine": "Command Line value",
      "integrityLevel": "String",
      "isElevated": true,
      "parentProcessCreatedDateTime": "2016-12-31T23:59:05.910252+00:00",
      "parentProcessId": 15,
      "parentProcessName": "Parent Process Name value",
      "processId": 9
    }
  ],
  "recommendedActions": [
    "Recommended Actions value"
  ],
  "registryKeyStates": [
    {
      "@odata.type": "microsoft.graph.registryKeyState",
      "hive": "String",
      "key": "Key value",
      "oldKey": "Old Key value",
      "oldValueData": "Old Value Data value",
      "oldValueName": "Old Value Name value",
      "operation": "String",
      "valueData": "Value Data value",
      "valueName": "Value Name value",
      "valueType": "String"
    }
  ],
  "severity": "String",
  "sourceMaterials": [
    "Source Materials value"
  ],
  "status": "String",
  "tags": [
    "Tags value"
  ],
  "title": "Title value",
  "triggers": [
    {
      "@odata.type": "microsoft.graph.alertTrigger",
      "type": "Type value",
      "value": "Value value"
    }
  ],
  "userStates": [
    {
      "@odata.type": "microsoft.graph.userSecurityState",
      "aadUserId": "Aad User Id value",
      "domainName": "Domain Name value",
      "emailRole": "String",
      "isVpn": true,
      "logonDateTime": "2016-12-31T23:57:12.5063859+00:00",
      "logonId": "Logon Id value",
      "logonIp": "Logon Ip value",
      "logonLocation": "Logon Location value",
      "logonType": "String",
      "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
      "userAccountType": "String",
      "userPrincipalName": "User Principal Name value"
    }
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState",
      "cve": "Cve value"
    }
  ]
}
```

