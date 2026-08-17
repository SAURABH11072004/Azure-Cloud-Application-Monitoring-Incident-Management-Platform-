# Azure Cloud Application Monitoring & Incident Management Platform

A cloud-based application monitoring and incident management platform built on **Microsoft Azure** to demonstrate practical skills in cloud architecture, application observability, identity and access management, incident detection, troubleshooting, and risk mitigation.

The project follows a production-oriented workflow:

**Requirements → Architecture → Deployment → Monitoring → Alerting → Incident Detection → Root Cause Analysis → Mitigation**

---

## 🚀 Project Overview

Modern applications require continuous monitoring to maintain availability, performance, security, and reliability.

This project provides a centralized platform for deploying a web application on Azure and monitoring its health using Azure-native services.

The platform enables teams to:

- Monitor application availability
- Track API requests and response times
- Detect application failures
- Monitor database dependencies
- Capture exceptions and application logs
- Generate alerts for abnormal conditions
- Investigate incidents
- Perform root-cause analysis
- Track incident resolution
- Apply technical mitigation strategies
- Control access using Microsoft Entra ID and Azure RBAC

---

## 🎯 Problem Statement

When applications are deployed to the cloud, simply hosting the application is not enough.

Engineering and operations teams need visibility into:

- Application availability
- API failures
- Response latency
- Database failures
- Dependency failures
- Authentication problems
- Application exceptions
- Infrastructure health
- Security-related events

Without centralized monitoring, identifying the root cause of an incident can become difficult and time-consuming.

### Proposed Solution

The proposed system combines Azure application hosting, monitoring, telemetry, identity management, and incident management into a single operational workflow.

```text
                         USERS
                           |
                           v
                    +-------------+
                    | React Web UI|
                    +-------------+
                           |
                         HTTPS
                           |
                           v
                +----------------------+
                |    Azure App Service |
                |  Node.js / Express   |
                +----------------------+
                     |            |
                     |            |
                     v            v
              +----------+   +--------------------+
              | Azure SQL|   | Application        |
              | Database |   | Insights           |
              +----------+   +--------------------+
                                  |
                                  v
                         +----------------+
                         | Azure Monitor  |
                         +----------------+
                           |            |
                           v            v
                       Metrics        Alerts
                           |            |
                           +-----+------+
                                 |
                                 v
                       Incident Dashboard
                                 |
                                 v
                       Root Cause Analysis
                                 |
                                 v
                            Mitigation




