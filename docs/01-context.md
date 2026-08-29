# 01 — Context and Problem

## Background

In December 2025, I assumed responsibility for the technical administration of the institutional Moodle platforms used by the ESGA.

At that time, two legacy Moodle environments were in operation. They were not duplicate platforms: each contained its own courses, teachers and students.

The objective was to understand the technical and operational limitations of the existing environments before defining a new platform.

## Assessment of the Legacy Environments

The assessment identified different problems across the existing environments.

### Legacy Platform 1

The platform presented functional problems, including password recovery not working correctly.

### Legacy Platform 2

The second environment was running Moodle 4.5.8 on shared hosting. The same server was also hosting the ESGA website, the Faculty website and the Observatory website.

The platform presented several problems:

- Password recovery was not working correctly.
- The messaging system was malfunctioning.
- Messages could contain unreadable characters.
- After using special characters, users could be unable to continue typing messages.
- The database contained an excessive amount of accumulated information, particularly in the question bank.
- Creating or restoring new courses could cause disproportionate database growth.
- Course creation/restoration processes could remain incomplete.
- The resulting database and process problems contributed to recurring server failures.

These conditions made it increasingly difficult to create new classrooms and maintain a stable environment.

## Investigation

The objective was not limited to correcting individual symptoms. The existing environments were investigated to determine the underlying causes of their failures and limitations.

The investigation included:

- Reviewing the infrastructure of both legacy platforms.
- Observing platform behavior under normal operation.
- Examining logs when failures occurred.
- Reviewing Moodle technical requirements.
- Investigating specific problems through Moodle documentation and community discussions.
- Reproducing relevant conditions in a laboratory environment when necessary.

This process allowed infrastructure and configuration decisions to be based on observed behavior rather than assumptions.

## Technical Findings

One of the existing platforms had a messaging problem for which a software-level workaround was identified through investigation of the Moodle community.

The workaround was reproduced and verified in the laboratory environment.

However, it was not applied to the existing production platform because the messaging problem was only one part of a broader set of infrastructure and database issues.

The investigation also showed that the shared hosting model was not appropriate for the expected evolution of the new platform.

The new environment would consolidate the courses, teachers and students previously distributed across the two legacy platforms. Therefore, the expected workload would be substantially greater than that of either individual platform.

Concurrent usage was also considered. Institutional assessments can generate high levels of simultaneous activity, making infrastructure capacity an important factor in platform stability.

## Requirements for the New Platform

The assessment led to several requirements for the new environment:

- Independent virtual server infrastructure.
- Current and supported operating system.
- Moodle version with a long-term support strategy.
- Resources sized according to expected workload and growth.
- Database engine compatible with the selected Moodle version.
- Web server configuration compatible with Moodle requirements.
- Deployment within the institutional Data Center.
- Laboratory validation before production deployment.
- Separation between production and experimental environments.

## Objective

The objective was to replace the legacy environments with a new Moodle platform capable of consolidating their users and courses while providing a more stable and maintainable technical foundation.

The solution was first designed and validated in a laboratory virtual machine.

The resulting environment was subsequently deployed as the production Moodle platform in the institutional Data Center.

## Approach

The project followed a problem-driven technical approach:

**Observe → Investigate → Test → Implement → Validate → Document**

Existing infrastructure, observed platform behavior, Moodle requirements and laboratory testing were used together to guide technical decisions.

Documentation and community resources were consulted when specific technical questions or implementation problems required verification.
