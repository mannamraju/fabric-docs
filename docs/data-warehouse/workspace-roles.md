---
title: Workspace roles
description: Learn about the roles you can use to manage user access within a workspace.
author: cynotebo
ms.author: cynotebo
ms.reviewer: wiassaf, jacindaeng
ms.date: 10/26/2023
ms.topic: conceptual
ms.custom: build-2023
ms.search.form: Warehouse roles and permissions, Workspace roles and permissions # This article's title should not change. If so, contact engineering.
---
# Workspace roles in Fabric data warehousing

**Applies to:** [!INCLUDE[fabric-se-and-dw](includes/applies-to-version/fabric-se-and-dw.md)]

This article details the permissions that workspace roles provide in [!INCLUDE [fabric-se](includes/fabric-se.md)] and [!INCLUDE [fabric-dw](includes/fabric-dw.md)]. For instructions on assigning workspace roles, see [Give Workspace Access](../get-started/give-access-workspaces.md).

[!INCLUDE [preview-note](../includes/preview-note.md)]

## Workspace roles

Assigning users to the various workspace roles provides the following capabilities:

| Workspace role   |  Description |
|---|---|
|**Admin**|Grants the user CONTROL access for each [!INCLUDE [fabric-dw](includes/fabric-dw.md)] and [!INCLUDE [fabric-se](includes/fabric-se.md)] within the workspace, providing them with full read/write permissions and the ability to manage granular user SQL permissions.<br/><br/>Allows the user to see workspace-scoped session, [monitor connections and requests in DMVs via TSQL](monitor-using-dmv.md), and [KILL](/sql/t-sql/language-elements/kill-transact-sql?view=fabric&preserve-view=true) sessions.|
|**Member**|Grants the user CONTROL access for each [!INCLUDE [fabric-dw](includes/fabric-dw.md)] and [!INCLUDE [fabric-se](includes/fabric-se.md)] within the workspace, providing them with full read/write permissions and the ability to manage granular user SQL permissions.|
|**Contributor**|Grants the user CONTROL access for each [!INCLUDE [fabric-dw](includes/fabric-dw.md)] and [!INCLUDE [fabric-se](includes/fabric-se.md)] within the workspace, providing them with full read/write permissions and the ability to manage granular user SQL permissions.|
|**Viewer**|Grants the user CONNECT and ReadData permissions for each [!INCLUDE [fabric-dw](includes/fabric-dw.md)] and [!INCLUDE [fabric-se](includes/fabric-se.md)] within the workspace. Viewers can be granted granular SQL permissions to read data from tables/views using T-SQL. For more information, see [Manage SQL granular permissions](sql-granular-permissions.md).|

## Related content

- [Security for data warehousing in Microsoft Fabric](security.md)
- [SQL granular permissions](sql-granular-permissions.md)
- [Row-level security in Fabric data warehousing](row-level-security.md)
- [Column-level security in Fabric data warehousing](column-level-security.md)
