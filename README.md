# QTC Workflow Queue (WFQ) — Administrator Application

> **Course:** CS3338 — Software Engineering  
> **Note:** This repository is a course project. Our team is using the QTC Workflow Queue (WFQ) project as a base template to demonstrate proficiency in software engineering tools including GitHub, Docker, Jira, TestRail, and LaTeX. The original SRS and SDD documents were produced by the QTC project team. Our contributions consist of toolchain setup, new feature additions, documentation updates, and testing artifacts added across each snapshot.

**Original Project:** QTC Workflow Queue (WFQ) Administrator Application by Leidos QTC Health Services  
**Course Team:** *(Add your group member names here)*  
**Project Timeframe:** 6 Months  
**Version:** 1.0 (Snapshot 1)

---

## Jira Board

> **[Click here to view the Jira Project Board](#)**  
> *(Replace `#` with your team's Jira board URL)*

---

## Project Objective

The QTC Workflow Queue (WFQ) Administrator Application is a web-based tool for authorized technical administrators to create, configure, and manage workflows used by the QTC WFQ system. It interacts directly with the existing WFQ SQL Server database and is built using ASP.NET Core MVC with C# and Entity Framework.

Our team is using this project as a structured template to practice the full software development lifecycle — from requirements and design documentation through implementation, testing, and deployment tooling.

### Snapshot 1 Goals
- Set up the repository structure and toolchain (GitHub, Docker, Jira, LaTeX)
- Review and adapt the existing SRS and SDD documents into LaTeX format
- Establish the base project framework and architecture
- Configure the ASP.NET Core MVC project with Entity Framework and SQL Server connectivity
- Implement the Authorization Module (URL query string flag-based access control)
- Build the core Workflow Dashboard UI (list, search, sort, paginate workflows)
- Implement Workflow Creation and Update functionality
- Set up Jira Sprint 1 with tasks derived from the existing requirements

---

## Why This Software Matters

Many organizations rely on manual, fragmented processes for workflow approvals — leading to miscommunication, data loss, and delays. The WFQ Administrator Application solves this by giving technical administrators a centralized, secure interface to define and manage the structure of the organization's workflow engine.

Key benefits:
- Replaces manual workflow configuration with a guided UI
- Enforces role-based access control to protect sensitive data
- Maintains a full audit trail of all administrative actions
- Supports HIPAA/HITECH compliance requirements

---

## Our Contributions (Course Project)

As a course team, our additions to this project across all snapshots include:

| Snapshot | Contribution |
|---|---|
| Snapshot 1 | Repository setup, LaTeX documentation, Docker scaffold, Jira Sprint 1 |
| Snapshot 2 | New feature addition, updated docs, TestRail Snapshot 2 report |
| Snapshot 3 | New feature addition, updated docs, TestRail Snapshot 3 report |
| Snapshot 4 | Final touches, future work reflection, TestRail Snapshot 4 report |

---

## Technology Stack

| Layer | Technology |
|---|---|
| Frontend | ASP.NET Core MVC (Razor Pages) |
| Backend | C# / .NET 7 |
| ORM | Entity Framework Core |
| Database | Microsoft SQL Server |
| Web Server | Internet Information Services (IIS) |
| IDE | Visual Studio 2022 |
| Source Control | Git / GitHub |

---

## How to Access / Run the Application

> **Note:** This application requires access to the QTC-managed SQL Server database instance. Contact your project administrator for connection credentials.

### Prerequisites
- [.NET 7 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/7.0)
- [Visual Studio 2022](https://visualstudio.microsoft.com/)
- [SQL Server Management Studio (SSMS) 19](https://learn.microsoft.com/en-us/ssms/install/install)
- Access to the WFQ SQL Server database (credentials provided by QTC)

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/your-org/wfq-admin.git
   ```
2. Open the solution in Visual Studio 2022.
3. Update the connection string in `appsettings.json` with your database credentials.
4. Build the solution:
   ```bash
   dotnet build
   ```
5. Run the application:
   ```bash
   dotnet run
   ```
6. Access the application in your browser at `https://localhost:5001?is_admin=true`

> **Authorization:** The application uses a URL query string flag (`?is_admin=true`) for administrative access. This flag is provided by the hosting environment in production.

---

## Repository Structure

```
/
├── README.md                        ← This file (User Manual)
├── docs/
│   ├── SDD.tex                      ← Software Design Document
│   ├── SRS.tex                      ← Software Requirements Specification
│   ├── DesignSpec.tex               ← Design Specification (page/component breakdown)
│   ├── SnapshotObjectives.tex       ← Snapshot objectives and reflections
│   └── WorkflowDiagram.png          ← High-level system workflow diagram
└── testrail/
    └── (TestRail reports added at Snapshot 2)
```

---

## Documents

| Document | Description |
|---|---|
| [SDD](docs/SDD.tex) | Software Design Document — architecture, components, database design |
| [SRS](docs/SRS.tex) | Software Requirements Specification — functional and non-functional requirements |
| [Design Spec](docs/DesignSpec.tex) | Breakdown of every page, screen, and component |
| [Snapshot Objectives](docs/SnapshotObjectives.tex) | Goals and reflections for each project snapshot |
| [Workflow Diagram](docs/WorkflowDiagram.png) | High-level diagram of system data flow |

---

## License

This project is developed for Leidos QTC Health Services as part of a senior design course engagement. All rights reserved.
