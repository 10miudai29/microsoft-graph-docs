---
title: "List members"
description: "Get the conversationMembers of a team."
author: "nkramer"
localization_priority: Priority
ms.prod: "microsoft-teams"
doc_type: apiPageType
---

# List members
Namespace: microsoft.graph

Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).

>Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|TeamMember.Read.All, TeamMember.ReadWrite.All|
|Delegated (personal Microsoft account) | Not supported.    |
|Application|TeamMember.Read.All, TeamMember.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.conversationmember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        }
    ]
}```
