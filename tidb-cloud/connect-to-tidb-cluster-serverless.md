---
title: Connect to Your TiDB Serverless Cluster
summary: Learn how to connect to your TiDB Serverless cluster via different methods.
---

# Connect to Your TiDB Serverless Cluster

This document introduces the methods to connect to your TiDB Serverless cluster.

> **Tip:**
>
> To learn how to connect to a TiDB Dedicated cluster, see [Connect to Your TiDB Dedicated Cluster](/tidb-cloud/connect-to-tidb-cluster.md).

After your TiDB Serverless cluster is created on TiDB Cloud, you can connect to it via one of the following methods:

- [Connect via private endpoint](/tidb-cloud/set-up-private-endpoint-connections-serverless.md) (recommended)

    Private endpoint connection provides a private endpoint to allow SQL clients in your VPC to securely access services over AWS PrivateLink, which provides highly secure and one-way access to database services with simplified network management.

- [Connect via public endpoint](/tidb-cloud/connect-via-standard-connection-serverless.md)

    The standard connection exposes a public endpoint with traffic filters, so you can connect to your TiDB cluster via a SQL client from your laptop.

    TiDB Serverless requires [TLS connections](/tidb-cloud/secure-connections-to-serverless-clusters.md), which ensures the security of data transmission from your applications to TiDB clusters.

- [Connect using built-in SQL Editor](/tidb-cloud/explore-data-with-chat2query.md)

    You can use AI-assisted SQL Editor in the [TiDB Cloud console](https://tidbcloud.com/) to run SQL quries. 

    In SQL Editor, you can either write SQL queries manually or simply press `Cmd + I` (or `Ctrl + I`) followed by your instructions to let AI generate SQL queries automatically, and then run SQL queries against databases without a local SQL client. You can find the query results in tables intuitively and check the query logs easily.

## What's next

After you have successfully connected to your TiDB cluster, you can [explore SQL statements with TiDB](/basic-sql-operations.md).
