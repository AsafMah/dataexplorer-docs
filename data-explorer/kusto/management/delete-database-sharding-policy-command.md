---
title: .delete database sharding policy command - Azure Data Explorer
description: This article describes the .delete database sharding policy command in Azure Data Explorer.
ms.reviewer: yonil
ms.topic: reference
ms.date: 10/10/2021
---
# .delete database sharding policy

Delete the database sharding policy. Use the [sharding policy](../management/shardingpolicy.md) to manage data sharding for databases and tables.  

The sharding policy defines if and how [Extents (data shards)](../management/extents-overview.md) in the Azure Data Explorer cluster should be sealed. When a database is created, it contains the default data sharding policy. This policy is inherited by all tables created in the database (unless the policy is explicitly overridden at the table level).

## Syntax

`.delete` `database` *DatabaseName* `policy` `sharding`

## Arguments

*DatabaseName* - Specify the name of the databse.

## Example

The following example deleted the sharding policy for a database:

```kusto
.delete database MyDatabase policy sharding 
```