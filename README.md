AZURE DATA FACTORY - DATA ENGINEERING PROJECT

PROJECT OVERVIEW
This repository provides Azure Data Factory solutions for enterprise-scale data integration. It includes hybrid connectivity, advanced scheduling, FTP/SFTP integration, incremental loading strategies, and robust error handling. The implementation supports secure and scalable production ETL pipelines.

KEY FEATURES

Self-hosted Integration Runtime (SHIR)
Secure hybrid connectivity between on-premises systems and Azure cloud services using authentication keys, firewall rules, and network security protocols. Enables movement of sensitive data across private and public networks while maintaining compliance.
Advanced Pipeline Scheduling and Automation
Supports custom scheduling patterns such as last Saturday of the month, cron expressions, and timezone-aware triggers. Pipelines can be configured for recurring reporting, batch data processing, and scheduled maintenance workflows.
FTP/SFTP Integration
Extracts and ingests data from external FTP and SFTP servers using secure transfer protocols. Supports various file formats (CSV, JSON, XML), file pattern matching, large file handling, and directory recursion. Enables integration with external partners and legacy systems.
Incremental Load Pipelines with Change Data Capture
Implements watermark-based incremental loading using high-water mark patterns and timestamp tracking. Optimizes pipeline performance by transferring only new or modified records, minimizing resource usage and maintaining data integrity.
Comprehensive Error Handling and Retry Logic
Incorporates robust error handling strategies including transient error detection, retry policies with exponential backoff, and dead-letter queue design patterns. Ensures operational stability and pipeline resilience with integrated alerting and monitoring.
TECHNICAL ARCHITECTURE

Data Sources

On-premises SQL Server
FTP/SFTP servers
REST APIs
Azure Blob Storage
Target Systems

Azure SQL Database
Azure Data Lake Storage
Azure Synapse Analytics
Azure Cosmos DB
Integration Components

Self-hosted Integration Runtime (SHIR) for hybrid connectivity
Azure Integration Runtime for cloud-native data transfers
Managed Virtual Network (VNet) for secure pipeline execution
Private endpoints for enhanced network isolation
SECURITY AND GOVERNANCE

Azure Key Vault for credential and secret management
Managed Identity authentication
Role-based access control (RBAC)
Data encryption in transit and at rest
TECHNOLOGIES AND SERVICES

Azure Data Factory
Self-hosted Integration Runtime
Azure SQL Database
Azure Key Vault
Azure Monitor
GitHub Actions (CI/CD integration)
