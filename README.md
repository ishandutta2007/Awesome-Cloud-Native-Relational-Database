# Awesome-Cloud-Native-Relational-Database

# Awesome-Cloud-Native-Relational-Database ☁️ 🗄️



<p align="center">

  <img src="assets/banner.svg" alt="Awesome Cloud Native Relational Database Banner" width="100%">

</p>



<p align="center">

  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>

  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>

  <a href="https://github.com/ishandutta2007/Awesome-Cloud-Native-Relational-Database"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Cloud-Native-Relational-Database?style=social" alt="GitHub_Stars"/></a>

  <a href="https://github.com/ishandutta2007/Awesome-Cloud-Native-Relational-Database/fork"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Cloud-Native-Relational-Database?style=social" alt="GitHub Forks"/></a>

  <a href="https://github.com/ishandutta2007/Awesome-Cloud-Native-Relational-Database/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Cloud-Native-Relational-Database?color=blue" alt="License"/></a>

  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

</p>



---



## 🌟 Top Cloud-Native Relational Database Ecosystem



**Curated List of Commercial Cloud Databases & Open-Source Distributed SQL Systems**  

*Focused on Serverless Postgres, Distributed SQL, HTAP Workloads, Multi-Region Replication & Self-Hosted Cloud-Native Databases*



**Last updated: October 2026** 📅



---



### 📌 Overview & SEO Summary

Welcome to the ultimate curated directory of **cloud-native relational database platforms**, **open-source distributed SQL systems**, and **serverless Postgres frameworks**. Whether you are looking for enterprise-grade commercial solutions (such as *Amazon Aurora*, *Google Cloud AlloyDB*, and *CockroachDB Cloud*), or self-hostable open-source alternatives (like *YugabyteDB*, *TiDB*, and *Neon*), this list covers category leaders, PostgreSQL compatibility, and privacy-respecting distributed data architectures.



**Key Market Context:**

- **PostgreSQL is the most portable relational engine** — available as managed service on all three major clouds with the strongest open-source ecosystem .

- **CockroachDB changed licensing** — now source-available with commercial license, free for companies under $10M revenue with mandatory telemetry .

- **Neon (serverless Postgres) was acquired by Databricks**, signaling consolidation in the serverless database space .



---



## 📑 Table of Contents

- [🏢 SaaS & Commercial Platforms](#-saas--commercial-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🛠️ How to Contribute](#%EF%B8%8F-how-to-contribute)

- [📊 Star History](#-star-history)

- [🤝 Support & Sponsorship](#-support--sponsorship)

- [⚠️ Disclaimer](#%EF%B8%8F-disclaimer)



---



## 🏢 SaaS / Commercial Platforms



The cloud-native relational database market is split between **hyperscaler managed services** (Aurora, AlloyDB, Spanner) that provide deep integration with their respective ecosystems, and **specialized distributed SQL platforms** (CockroachDB, YugabyteDB, TiDB) that offer multi-cloud portability. For a typical production workload (4 vCPUs, 16 GB RAM, 500 GB storage, Multi-AZ), **Aurora PostgreSQL costs $600–$800/month** while **AlloyDB runs $550–$750/month** . **Neon** charges **$0.106/CU-hour** after its free tier, with compute suspended at zero cost .



| SaaS / Commercial Platform | Company / Owner | Valuation / Market Cap | Standard Edition Starting Price | Free Tier / Free Trial Limits | Description |

| :--- | :--- | :--- | :--- | :--- | :--- |

| **[Amazon Aurora](https://aws.amazon.com/rds/aurora/)** ☁️ | Amazon | ~$2.0 Trillion | **$600–$800/month** (4 vCPU, 16 GB, 500 GB Multi-AZ)  | **Free tier: 750 hours of db.t3.medium for 12 months** | **AWS-native cloud database** — PostgreSQL and MySQL compatible with **storage auto-scaling and replication**. Aurora Serverless v2 for variable workloads. **High portability for data** (standard PostgreSQL wire protocol) but Aurora-specific functions create some lock-in . |

| **[Google Cloud AlloyDB](https://cloud.google.com/alloydb)** 🌐 | Google (Alphabet) | ~$2.0 Trillion | **$550–$750/month** (4 vCPU, HA instance)  | **$300 free credits** for new customers | **GCP-native PostgreSQL-compatible database** — **Columnar engine for analytics**, AI-assisted tuning, and **99.99% availability SLA**. PostgreSQL wire compatible for maximum portability . |

| **[CockroachDB Cloud](https://www.cockroachlabs.com/)** 🪳 | Cockroach Labs | Private | **$0.092/vCPU-hour** (~$203/month for 2 vCPU, 100 GB)  | **30-day trial with $400 credit** (no permanent free tier for new orgs)  | **Distributed SQL database** — **Automatic sharding, multi-region deployment, and Raft consensus replication** . **Serializable isolation by default** (stronger than MySQL's repeatable read). **PostgreSQL wire compatible** — most tools work directly . **License change**: now source-available with commercial license, free for companies under $10M revenue with mandatory telemetry . |

| **[PlanetScale](https://planetscale.com/)** 🪐 | PlanetScale | Private | **Custom pricing** | **Hobby: free tier available** | **MySQL-compatible serverless database** — Built on **Vitess** for horizontal scaling of MySQL. **HTTP protocol access** for edge and serverless environments . **Non-blocking schema changes** and database branching workflows. |

| **[YugabyteDB Managed (Aeon)](https://www.yugabyte.com/)** 🐘 | Yugabyte | Private | **$125/vCPU/month** (Aeon)  | **Sandbox: free up to 2 vCPU, 4 GB memory, 10 GB storage** (not for production, 15 connection limit)  | **Distributed PostgreSQL-compatible database** — **Reuses PostgreSQL query layer** with ~85% compatibility . **Apache 2.0 licensed core** (unlike CockroachDB's source-available license) . **Row store (YSQL) + column store analytics** unified platform. Supports stored procedures, triggers, and extensions . |

| **[Neon](https://neon.tech/)** ⚡ | Databricks | Private (Acquired) | **$0.106/CU-hour** (Launch plan, pay-as-you-go)  | **Free plan: 100 CU-hours/project, 0.5 GB storage, autoscaling to 2 CU**  | **Serverless PostgreSQL** — **Compute scales to zero when idle** (suspended compute costs $0). **Instant branching and bottomless storage**. **Single primary** — not for multi-region writes . **Acquired by Databricks** . |

| **[SingleStore](https://www.singlestore.com/)** 🎯 | SingleStore | Private | **Custom enterprise pricing** (freemium tier available)  | **Free tier available** | **Distributed SQL with built-in vector search** — **Row store + column store in one database** for HTAP workloads. **MySQL and MongoDB wire protocol compatibility**. Multiple vector index types (HNSW, IVF). **Proven at scale with 100+ Fortune 500 customers** . |

| **[TiDB Cloud](https://www.pingcap.com/tidb-cloud/)** 🔷 | PingCAP | Private | **Starter: Free**; **Essential: ~$20/day for small production**  | **Free: 25 GiB row storage, 25 GiB column storage, 250M RUs/month**  | **Open-source HTAP database** — **MySQL protocol compatible**. **TiKV (row store) + TiFlash (column store)** for simultaneous transaction and analytics . **Apache 2.0 licensed**. Transparent horizontal scaling. **Architecture complexity requires distributed systems knowledge** . |

| **[Supabase](https://supabase.com/)** 🟢 | Supabase | Private | **Pro: $25/month** | **Free: 2 projects, 500 MB database, 1 GB storage** | **Open-source Firebase alternative** — **PostgreSQL with real-time subscriptions, auth, and edge functions** . **HTTP client via PostgREST** endpoints. **pgvector hosting** for AI applications . |

| **[Azure Cosmos DB](https://azure.microsoft.com/en-us/products/cosmos-db/)** 🔵 | Microsoft | ~$3.90 Trillion | **$12–$18/day** (autoscale 400–4000 RU/s, 100 GB storage)  | **Free tier: 1000 RU/s + 25 GB permanent**  | **Multi-model globally distributed database** — **Document, key-value, graph, and wide-column APIs**. **5 consistency levels selectable** . **Turnkey global distribution**. **Higher price and more complex configuration** than relational-only alternatives . |



---



## 🔓 Open-Source GitHub Projects



*Sorted by GitHub_Stars_Count (Descending)* 🌟



- **[TiDB](https://github.com/pingcap/tidb)** [![Stars](https://img.shields.io/github/stars/pingcap/tidb?style=social&color=white)](https://github.com/pingcap/tidb/stargazers)  

  **Open-source distributed SQL database**, Apache-2.0 licensed. **The most popular open-source HTAP database** . **MySQL protocol compatible** — horizontal scaling transparent to applications. **TiKV (row store) + TiFlash (column store)** serve transactional and analytical workloads from one data copy . **Raft consensus for strong consistency and high availability**. **Architecture complexity**: PD/TiKV/TiFlash components require distributed systems expertise — **overkill for small workloads** . **Note**: Compatible with MySQL, not PostgreSQL . 🚀



- **[YugabyteDB](https://github.com/yugabyte/yugabyte-db)** [![Stars](https://img.shields.io/github/stars/yugabyte/yugabyte-db?style=social&color=white)](https://github.com/yugabyte/yugabyte-db/stargazers)  

  **Distributed PostgreSQL-compatible database**, Apache-2.0 licensed. **The most faithful PostgreSQL distributed variant** — **reuses PostgreSQL query layer (YSQL) with ~85% compatibility** . **Stored procedures, triggers, and extensions work** — unlike many distributed alternatives. **Pure Apache 2.0 license** (no revenue caps or telemetry requirements, unlike CockroachDB) . **Automatic replication and failover**, independent scaling of storage and compute. **Row store (YSQL) + column store analytics** unified . **Limitation**: Currently based on PostgreSQL 15 (three major versions behind PostgreSQL 18), and ecosystem maturity is far behind standalone PostgreSQL . 🐘



- **[CockroachDB](https://github.com/cockroachdb/cockroach)** [![Stars](https://img.shields.io/github/stars/cockroachdb/cockroach?style=social&color=white)](https://github.com/cockroachdb/cockroach/stargazers)  

  **Distributed SQL database with automatic sharding and multi-region support**, Source-available (BSL/Commercial) licensed. **Raft consensus replication** — survives data center failures without manual failover . **Automatic rebalancing** — add nodes to scale horizontally without application sharding . **Serializable isolation by default** (stronger than MySQL's repeatable read) . **PostgreSQL wire compatible** — most tools work directly . **Data geo-partitioning** for GDPR compliance . **License caveat**: Now source-available with commercial restrictions — free for companies under $10M revenue with **mandatory telemetry that cannot be disabled** . **Distributed consensus adds write latency** — single-node PostgreSQL is faster for small workloads . 🪳



- **[PostgreSQL](https://github.com/postgres/postgres)** [![Stars](https://img.shields.io/github/stars/postgres/postgres?style=social&color=white)](https://github.com/postgres/postgres/stargazers)  

  **The world's most advanced open-source relational database**, PostgreSQL License (similar to MIT). **The strongest open-source relational ecosystem** — JSONB, arrays, full SQL standard, window functions, CTEs, materialized views . **PostGIS, TimescaleDB, pgvector** extensions for geospatial, time-series, and AI workloads . **PostgreSQL 18** (September 2025) adds async I/O (io_uring) for up to **3x I/O-intensive speedup**, multi-core parallel query, and logical replication with per-table granularity . **Most portable relational engine** — available as managed service on all major clouds with standard wire protocol . **Trade-off**: More tuning required than MySQL for initial setup . **The foundation for most open-source cloud-native databases** — Aurora, AlloyDB, YugabyteDB, and Neon all build on PostgreSQL. 🐘



- **[MariaDB](https://github.com/MariaDB/server)** [![Stars](https://img.shields.io/github/stars/MariaDB/server?style=social&color=white)](https://github.com/MariaDB/server/stargazers)  

  **Community-developed MySQL fork**, GPL-2.0 licensed. **Created by MySQL's original developers** after Oracle acquisition . **Galera Cluster for true multi-master synchronous replication** (MySQL is single-master topology) . **ColumnStore analytics engine** and **11.8 LTS with built-in vector search** (June 2025) for AI applications . **Community-driven feature development** — features serve users, not commercial interests . **Missing**: MySQL 8.0's document store API . 🔄



- **[Percona Server for MySQL](https://github.com/percona/percona-server)** [![Stars](https://img.shields.io/github/stars/percona/percona-server?style=social&color=white)](https://github.com/percona/percona-server/stargazers)  

  **Enhanced MySQL drop-in replacement**, GPL-2.0 licensed. **Fully compatible with MySQL** while adding enterprise capabilities . **ThreadPool** improves high-concurrency performance. **Hot backup without blocking backup locks**. **PAM authentication** and **InnoDB performance improvements**. **Best for teams wanting "better MySQL" without changing ecosystems** — compatibility is more conservative than MariaDB's aggressive feature additions . ⚙️



- **[SQLite](https://github.com/sqlite/sqlite)** [![Stars](https://img.shields.io/github/stars/sqlite/sqlite?style=social&color=white)](https://github.com/sqlite/sqlite/stargazers)  

  **Embedded relational database**, Public Domain. **Zero configuration, no server process, entire database in one file** . **Backup/migration/version management is just file copy**. **Tiny memory footprint** — first choice for resource-constrained environments. **No client-server capability** — network access requires wrapping . **The most deployed database in the world** — present in every smartphone, browser, and countless applications. 📱



- **[Turso](https://github.com/tursodatabase/libsql)** [![Stars](https://img.shields.io/github/stars/tursodatabase/libsql?style=social&color=white)](https://github.com/tursodatabase/libsql/stargazers)  

  **SQLite-compatible database for scalable multi-tenant applications**, MIT licensed. **17,215+ stars** . **Simple developer experience with SQLite compatibility** — build and scale multi-tenant applications with **unlimited databases** . **Designed for edge and serverless deployments**. 🌐



- **[Databend](https://github.com/datafuselabs/databend)** [![Stars](https://img.shields.io/github/stars/datafuselabs/databend?style=social&color=white)](https://github.com/datafuselabs/databend/stargazers)  

  **Cloud-native data warehouse for lightning-fast analytics**, Apache-2.0 licensed. **9,440+ stars** . **Elastic cloud data warehouse** built for high-performance analytics. **Seamless integration with popular data tools**. 📊



---



## 🛠️ How to Contribute



Contributions are welcome! Follow these steps to submit new cloud-native databases or open-source distributed SQL software:



1. 🍴 **Fork** the repository.

2. 📝 **Add/edit** entries in `README.md` maintaining table/list structure and formatting.

3. 🔗 Include project title, official website/GitHub link, exact Stars_Count, license, and brief description.

4. 🚀 Submit a **Pull Request** with a descriptive summary of your changes.



---



## 📊 Star History



[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Cloud-Native-Relational-Database&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Cloud-Native-Relational-Database&type=date&legend=top-left)



---



## 🤝 Support & Sponsorship



If you find this cloud-native relational database repository useful, please consider supporting the project:



- ⭐ **Star** this repository to increase visibility!

- 🔀 **Fork** and share with fellow database engineers, platform architects, and open-source advocates.

- ☕ **Sponsor & Buy Me a Coffee**: Support ongoing open-source curation via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).



---



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement. ℹ️

- **CockroachDB's licensing changed significantly** — now source-available with commercial restrictions. Free for companies under **$10M revenue**, but with **mandatory telemetry that cannot be disabled** . New Cloud organizations get a **30-day trial with $400 credit** instead of a permanent free tier . **YugabyteDB remains pure Apache 2.0** with no revenue caps .

- **Do not choose distributed SQL unless you have a real need** — CockroachDB, TiDB, and YugabyteDB add complexity (quorum, replication zones, distributed consensus) and write latency compared to single-node PostgreSQL . **For sub-terabyte workloads with moderate growth, single-node PostgreSQL is simpler and sufficient** .

- **PostgreSQL compatibility varies by database**: **YugabyteDB is ~85% compatible** (based on PG 15) , **CockroachDB is wire-compatible** but lacks some PostgreSQL features , and **TiDB is MySQL-compatible, not PostgreSQL** .

- **Cloud database costs are driven by compute, storage, I/O, and data transfer** — direct comparison across providers is challenging. **Use Performance Insights (AWS), Query Performance Insight (Azure), or Query Insights (GCP) to identify right-sizing opportunities** .

- **Open-source databases are not turnkey** — **TiDB requires distributed systems expertise** (PD/TiKV/TiFlash components) . **Always validate with a proof-of-concept** and test failover/recovery procedures before production deployment. 🗄️



---



<p align="center">

  <b>Made with ❤️ for database engineers, platform architects, and open-source cloud-native database advocates.</b>

</p>
