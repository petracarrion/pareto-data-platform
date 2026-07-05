---
title: Pareto Data Platform
author: Petra Carrión
theme: uncover
class:
  - invert
transition: slide
paginate: true
backgroundImage: url('dark-background.jpg')
---

# Pareto Data Platform

## What is it?

The Pareto Data Platform is an architecture blueprint for a data platform that fits 80% of the needs of medium size
company with just a 20% of complexity

<!-- HTML comment recognizes as a presenter note per pages. -->
<!-- You may place multiple comments in a single page. -->

---

## Assumptions

- The main use case for the data platform is Business Intelligence
- The company already use Microsoft Services, especially Microsoft Entra ID
- The major data sources run on-premise

---

## Components

The Pareto Data Platform is composed of:

- Azure Data Factory as ETL Tool
- Azure Data Lake as Persistent Staging Area
- Azure Synapse Dedicated SQL Pool as Data Warehouse
- Microsoft Power BI as BI Tool

---

## Azure Data Factory as ETL Tool

Azure Data Factory is a cloud-based data integration service that enables you to automate data movement and
transformation

Combined with Microsoft Integration Runtime, we will have an enterprise-grade ETL tool capable of extracting data from
applications and databases running on-premises

---

## Azure Data Lake as Persistent Staging Area

<style scoped>section{font-size:32px;}</style>

Azure Data Lake extends the capabilities of Azure Blob Storage to support hierarchical role-based access control while
it remains extremely cost-effective

Using such as simple API and plain file-based storage will help us stay vendor-neutral and be able to migrate to any
other cloud provider in the future

Storing the data in the Azure Data Lake before moving it to the data warehouse will create an additional backup layer

---

## Azure Synapse Dedicated SQL Pool as Data Warehouse

<style scoped>section{font-size:32px;}</style>

Azure Synapse Dedicated SQL Pool is a fully managed elastic data warehouse that provides a scalable and cost-effective
solution for storing and analyzing large volumes of data

The reason to use a Dedicated SQL Pool instead of the Serverless alternative is the higher performance and improved cost
transparency

The Serverless SQL Pool might be a better choice for smaller workloads or sporadic data analysis but we assume
uninterrupted usage by our BI users during working hours