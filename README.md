# Institutional Moodle Platform

Technical documentation of the design, deployment, migration and ongoing operation of an institutional Moodle platform.

## Overview

This project documents the technical work involved in consolidating two existing Moodle environments into a new independent platform, from the initial infrastructure assessment through laboratory validation, production deployment and subsequent maintenance.

The project originated from the analysis of existing platforms with recurring functional, database and infrastructure issues that affected their stability and ability to evolve.

The new environment was designed and validated in a laboratory VM before being deployed in the institutional Data Center.

## Technical Scope

The project includes:

- Infrastructure assessment and requirements analysis
- Moodle version selection
- Operating system and platform requirements
- Virtual machine design and resource sizing
- Web server and database configuration
- Laboratory environment and compatibility testing
- Moodle deployment
- Migration of courses and users
- Database and question bank cleanup
- Troubleshooting and root cause analysis
- Production deployment
- Ongoing platform maintenance and technical support
- Development of scripts for operational checks
- Laboratory experiments and technology evaluation

## Approach

The platform was developed through an iterative, problem-driven approach:

**Observe → Investigate → Test → Implement → Validate → Document**

Existing platform behavior, infrastructure conditions and operational requirements were used to guide technical decisions. Documentation and community resources were consulted when specific issues required further verification.

## Project Status

**Production — Operational and maintained**

The laboratory environment is also retained as a safe environment for testing changes and exploring alternative configurations without affecting production.

## Documentation

Detailed documentation is organized by project stage:

- [Context and Problem](docs/01-context.md)
- Architecture and Technical Decisions
- Laboratory Validation
- Deployment
- Migration
- Operations and Maintenance
- Technical Experiments

## Note

This repository documents the technical aspects of the project while omitting institutional, infrastructure and operational information that is not intended for public disclosure.

