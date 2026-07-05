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
- Azure Synapse as Data Warehouse
- Microsoft Power BI as BI Tool

---

## Azure Data Factory as ETL Tool

Azure Data Factory is a cloud-based data integration service that enables you to automate data movement and
transformation.

Combined with Microsoft Integration Runtime, we will have an enterprise-grade ETL tool capable of extracting data from
applications and databases running on-premise.
