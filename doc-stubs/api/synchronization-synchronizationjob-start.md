---
title: "synchronizationJob: start"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# start
Namespace: microsoft.graph

**TODO: Add Description**

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
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/start
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|parameters|[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [stringKeyStringValuePair](../resources/synchronization-stringkeystringvaluepair.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/start

Content-Type: application/json
Content-length: 122

{
  "parameters": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
    }
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.stringkeystringvaluepair"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.graph.stringKeyStringValuePair"
  }
}
```

