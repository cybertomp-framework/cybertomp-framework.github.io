---
layout: page
title: CyberTOMP® versioning
subtitle: Controlling the evolution of the framework
cover-img:
  - "/assets/img/section-cover.png"
---

This section describes how versions of the **CyberTOMP®** framework and its associated projects are defined, aligned, and maintained over time. The goal is to ensure consistency, stability, and traceability across all components of the framework, while allowing controlled evolution and coordinated releases.

### Project Naming Convention

To ensure clarity and uniformity:

* All projects belonging to the **CyberTOMP®** framework must follow the naming format
  **`cybertomp-project-name`**.
* Examples include:

  * `cybertomp-framework-core`
  * `cybertomp-fleco`
  * `cybertomp-fleco-studio`

### 2. Core Framework Project

* The project **`cybertomp-framework-core`** represents the **CyberTOMP®** framework itself.
* It is the **main reference project**, and all other subprojects must align with it.
* The version of `cybertomp-framework-core` defines the **official version of the CyberTOMP® model**.

### 3. Versioning Scheme

#### 3.1 Framework Core Versioning

* The `cybertomp-framework-core` project follows the pattern:
  **`cybertomp-framework-core-version`**
* No revision number is included.
* A new version is released **only when major changes are introduced** that may break compatibility or require realignment across projects.
* Example:

  * `cybertomp-framework-core-1` → **CyberTOMP® version 1**
  * `cybertomp-framework-core-2` → **CyberTOMP® version 2**
* The core framework is expected to evolve **more slowly and conservatively** than other projects.

#### 3.2 Subproject Versioning

* All other projects must follow the pattern:
  **`project-version.revision`**
* Where:

  * **version** matches the corresponding `cybertomp-framework-core` version.
  * **revision** is an incremental number for bug fixes or enhancements that remain fully compatible with the same framework version.
* Examples:

  * `cybertomp-fleco-studio-1.4`
  * `cybertomp-fleco-1.0`
    Both are aligned with **CyberTOMP® version 1** (`cybertomp-framework-core-1`).

### 4. Mapping Between Framework and Model Versions

The version of `cybertomp-framework-core` determines the official **CyberTOMP® model version**:

* **CyberTOMP® version 1** ⇔ `cybertomp-framework-core-1`
* **CyberTOMP® version 2** ⇔ `cybertomp-framework-core-2`
* **CyberTOMP® version 3** ⇔ `cybertomp-framework-core-3`

### 5. Coordinated Releases and Consistency

* All projects must remain **fully consistent** with the framework version they share.
* When a new **CyberTOMP® framework version** is released:

  * All subprojects must be updated, tagged, and released simultaneously.
  * Subprojects will be released as `project-version.0`, indicating alignment with a new framework version.
* A new version of `cybertomp-framework-core` **cannot be released** unless all other projects are updated accordingly.

### 6. Branching Strategy

Each project repository must include at least the following branches:

* **`master`**
  Represents the latest stable release. Minimal activity.
* **`dev-current`**
  Bug fixes and minor changes targeting new revisions of the current framework version.
* **`dev-next`**
  Developments intended for the next major version of the CyberTOMP® framework.

Additional branches may be created when needed, but they must be **temporary** and merged or removed once their purpose is fulfilled.

### 7. Version Freezing Policy

* Once a new **CyberTOMP® framework version** is released:

  * Previous versions become **frozen**.
  * They remain available for reference, use, and download.
  * No further contributions, corrections, or evolutions are accepted.

### 8. Governance and Compatibility

* The **Steering Committee** coordinates the joint release process across all projects, ensuring synchronization, stabilization, and readiness.
* **Backward compatibility** is considered whenever feasible.
* All releases and their corresponding changes are publicly documented in the
  **[Releases](/releases)** section.

