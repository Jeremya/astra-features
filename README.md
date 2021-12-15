# AstraDB features

## TL;DR
AstraDB is the Serverless SaaS offering from DataStax built on Apache Cassandra™ running on Kubernetes, available in three public cloud providers (GCP, AWS and Azure) and multi-region.

https://docs.astra.datastax.com/docs/what-is-datastax-astra

Note: Astra has recently migrated all offerings to Serverless only. This document therefore
does not cover the obsolete Classic Astra.

## Not Yet Supported
* BYOK: Bring Your Own Key

# Product
## Offerings
https://astra.datastax.com

## Pricing
Astra pricing has the following units of measure:
* Read and write requests (per 1M)
* Data storage (GB/month)
* Data transfer (GB/month) Also the cloud provider and region selected affects the price of each unit of measure.

Read and write requests, including API calls, are measured and charged monthly in increments of one million. Data storage and transfer are measured separately; each data type is charged monthly in increments of one GB.

There are options of savings depending on the minimum monthly spend.

For more details: https://docs.datastax.com/en/astra/docs/pricing-and-billing.html

## Security
* Private Endpoint: AstraDB provides a private channel between your VPC and Astra DB to improve security and latency.
* Encryption at Rest: all Astra DB data is encrypted at rest.
* IP Access Lists: configure IPs, CIDR blocks that can access Astra DB hosted resources - REST, GraphQL endpoints, Swagger, CQLsh.
* Encryption in Transit: all the internal and external communications to Astra DB use TLS with mutual authentication enabled.



## Scalability
* AstraDB Serverless auto scales according to the demand (Read/Write Capacity Units). This operation is transparent.
* Note that by default AstraDB workloads are limited to 4096 ops/sec by default. In order to increase the limit, a support ticket must be raised ("Rate limit reached" error).

