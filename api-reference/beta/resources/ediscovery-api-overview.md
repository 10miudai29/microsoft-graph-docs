---
title: "Use the Microsoft Graph eDiscovery API"
description: " > **Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported."
localization_priority: Priority
author: ""
ms.prod: "eDiscovery"
doc_type: resourcePageType
---

# Use the Microsoft Graph Compliance API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The Microsoft 365 eDiscovery APIs provide functionality for organizations to automate repetitive tasks, integrate with their existing eDiscovery tools to build a repeatable workflows that may be required based on industry regulations.  The eDiscovery APIs should be used to aid your legal needs.

> [!IMPORTANT]
> The eDiscovery APIs are intended for the use of eDiscovery operations for Litigation, Investigation and regulatory requests. These APIs should not be used as a substitute for journaling data out of the Microsoft 365 system or any other mass download.

The Microsoft 365 eDiscovery Graph API includes the following key entities.

| Name | Type       | Use case |
|:-|:-|:-|
| eDiscovery case | [ediscoveryCase](ediscovery-case.md) | eDiscovery cases are the container for all eDiscovery objects including custodians, holds, searches, review set and exports. |
| eDiscovery review set| [reviewSet](ediscovery-reviewset.md) | eDiscovery review sets are static set of electronically stored information collected for use in a litigation, investigation or regulatory request. |
| eDiscovery review set query | [reviewSetQuery](ediscovery-reviewset-query.md) | eDiscovery review set queries are used to discover, cull, review and tag [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure)) with the ultimate goal of production to the requestor or opposing counsel.

## What's new

Find out about the [latest new features and updates](/graph/whats-new-overview) for these API sets.