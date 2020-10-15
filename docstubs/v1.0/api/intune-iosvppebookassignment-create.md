---
title: "Create iosVppEBookAssignment"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create iosVppEBookAssignment

Namespace: microsoft.graph

Create a new iosVppEBookAssignment object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request Body

In the request body, supply JSON representation of the [iosVppEBookAssignment](../resources/intune-iosvppebookassignment.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create an iosVppEBookAssignment object.

| Property | Type | Description |
| :------- | :--- | :---------- |

## Response

If successful, this method returns a `201 Created` response code and an iosVppEBookAssignment object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_iosvppebookassignment"
}
-->

```http
POST https://graph.microsoft.com/v1.0

Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "installIntent": "String",
  "target": {
    "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.iosVppEBookAssignment"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String(identifier)",
  "installIntent": "String",
  "target": {
    "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}
}

```