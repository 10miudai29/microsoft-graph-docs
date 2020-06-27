---
title: "Update aadUserConversationMember"
description: "Update the properties of an aadUserConversationMember object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update aadUserConversationMember
Namespace: microsoft.graph

Update the properties of an [aadUserConversationMember](../resources/aaduserconversationmember.md) object.

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
PATCH /aadUserConversationMember
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [aadUserConversationMember](../resources/aaduserconversationmember.md) object.

The following table shows the properties that are required when you create the [aadUserConversationMember](../resources/aaduserconversationmember.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|roles|String collection|**TODO: Add Description** Inherited from [conversationMember](../resources/conversationmember.md)|
|displayName|String|**TODO: Add Description** Inherited from [conversationMember](../resources/conversationmember.md)|
|userId|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [aadUserConversationMember](../resources/aaduserconversationmember.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_aaduserconversationmember"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/aadUserConversationMember
Content-Type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "userId": "String",
  "email": "String"
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
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "44aca988-a988-44ac-88a9-ac4488a9ac44",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "userId": "String",
  "email": "String"
}
```

