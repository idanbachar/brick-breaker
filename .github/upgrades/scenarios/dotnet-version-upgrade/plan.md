# .NET Version Upgrade Plan

## Overview

**Target**: Upgrade the Brick Breaker solution to .NET 10 and update dependencies to latest supported stable versions.
**Scope**: Single SDK-style WinForms project with low upgrade complexity.

### Selected Strategy
**All-At-Once** — All projects upgraded simultaneously in a single operation.
**Rationale**: 1 project on modern .NET (net8.0), no dependency tiers, no API-breaking issues reported in assessment.

## Tasks

### 01-solution-upgrade: Upgrade project framework and dependencies

Upgrade the project target framework to net10.0-windows and update package references to the latest supported stable versions for the new framework. Then restore, build, and run tests to validate the upgrade end-to-end in one atomic pass.

**Done when**: The project targets net10.0-windows, package references are updated to supported stable versions, restore/build succeed, and available tests pass.

---
