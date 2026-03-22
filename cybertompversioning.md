---
layout: page
title: CyberTOMP® Versioning, Naming and Release Policy
subtitle: Controlling the evolution of the framework
cover-img:
  - "/assets/img/section-cover.png"
---

## 1. Ecosystem Overview

CyberTOMP® is developed as an **ecosystem of coordinated projects** hosted under the GitHub organization **[cybertomp-framework](https://github.com/cybertomp-framework){:target="_blank"}**

The ecosystem includes:

- The **CyberTOMP® model and framework specification**.
- The **Official supporting software**.
- The **project web site**.

Each component is maintained in a **separate repository**, while the ecosystem evolves through **coordinated releases**.

The main project portal and documentation site can be accessed via **[https://cybertomp.org](https://cybertomp.org)**:

This site acts as the **entry point for the entire CyberTOMP® ecosystem**, providing documentation, release information, and links to all repositories.

## 2. Project Naming Convention

All official repositories belonging to the CyberTOMP® ecosystem follow the naming pattern:

```
cybertomp-<component>
```

Examples:

```
cybertomp-framework-core
cybertomp-fleco-library
cybertomp-fleco-studio
cybertomp-framework.github.io
```

This naming convention ensures that CyberTOMP® components are clearly identifiable and consistently organized within the GitHub organization.

## 3. Ecosystem Versioning

CyberTOMP® uses a **single version number for the entire ecosystem**.

A version represents a **coherent and fully aligned state** of:

- The CyberTOMP® model and framework specifications.
- The official supporting software.  
- The framework web site.  

Examples:

```
CyberTOMP® v1
CyberTOMP® v2
CyberTOMP® v3
```

All repositories participating in a given release share the **same version tag**.

Example:

```
cybertomp-framework-core      v2
cybertomp-fleco-library       v2
cybertomp-fleco-studio        v2
cybertomp-framework.github.io v2
```

This approach guarantees compatibility across the ecosystem and simplifies version management.

## 4. Repository Version Tags

Repositories do not maintain independent major versions.

Instead, they publish **tags aligned with the ecosystem version**:

```
v1
v2
v3
```

A repository tagged with `v2` is part of the **CyberTOMP® v2 ecosystem release**.

Minor fixes or internal improvements may occur between releases but remain associated with the same ecosystem version.

## 5. Named Releases

In addition to the numeric version, each CyberTOMP® release may include a **release name**.

Release names provide a human-friendly way to refer to ecosystem versions and help distinguish major milestones in the project evolution. All release names in CyberTOMP®, if defined, will be star names in ascending alphabetical order.

Example:

```
CyberTOMP® v1 – Aldebaran
CyberTOMP® v2 – Betelgeuse
CyberTOMP® v3 – ...
```

Release names are optional but recommended for major versions of the ecosystem.

They are primarily used in:

- Documentation.  
- Presentations.  
- Publications.  
- Roadmap communication.  

However, the numeric version remains the **canonical technical identifier**.

## 6. Ecosystem Releases

A new CyberTOMP® version (as a whole) is released when significant changes occur in the model that make backward compatibility unfeasible and this changes require coordinated updates across projects.

An ecosystem release consists of:

1. Creating a new version tag across participating repositories.  
2. Publishing release notes. 
3. Updating the project portal and documentation.  
4. Update branches in all repositories.  

Example:

```
CyberTOMP® v2 – Betelgeuse
```

Repositories included in the release:

```
cybertomp-framework-core  
cybertomp-fleco-library  
cybertomp-fleco-studio   
cybertomp-framework.github.io  
```

Each repository publishes the corresponding tag:

```
v2
```

This guarantees alignment and compatibility across the ecosystem.

## 7. Development Branching Model

CyberTOMP® repositories follow a **three‑branch model** designed to support coordinated releases, maintain historical reproducibility, and minimize long‑term maintenance overhead.

### Branches

| Branch          | Purpose |
|-----------------|---------|
| `master`        | Latest stable version. |
| `next`          | Development of the upcoming version. |
| `release/vX`    | Frozen branch for version **vX**, used only for critical bugfixes. |

### Branch Workflow

1. **Development occurs in `next`**  
   All new features, improvements, and changes targeting the next major ecosystem version are committed to the `next` branch.

2. **Publishing a new ecosystem release**  
   When a new version *vX* is ready:
   - `next` is merged into `master`.
   - `master` is tagged as `vX`.
   - A new branch `release/vX` is created from `master`.
   
3. **Role of `master`**  
   After a release, `master` represents the **current stable version** and remains unchanged until the next release.

4. **Role of `release/vX` branches**  
   Each `release/vX` branch:
   - Represents a **frozen snapshot** of version *vX*.
   - Accepts **only critical bugfixes** for a period of **6 months** after its creation.
   - Generates incremental maintenance tags (`vX.1`, `vX.2`, …) when fixes are applied.
   - Remains permanently available for historical reference, even after the maintenance window closes.

5. **No merges between release branches and main/next**  
   - Fixes applied to `release/vX` **are not merged back** into `master` or `next`.
   - If a fix is also relevant for future versions, it must be applied **manually** to `next`.

This model ensures clean separation between past, present, and future development lines.

## 8. Version Lifecycle

Once a new ecosystem version is released:

- The previous version becomes **frozen**.  
- A `release/vX` branch is created to preserve it.  
- Only **critical bugfixes** are accepted for the next **6 months**.  
- After 6 months, the branch remains available but receives **no further changes**.  
- Development continues exclusively in `next` toward the next ecosystem version.  

This lifecycle ensures stability, reproducibility, and minimal maintenance burden while preserving the full historical evolution of the ecosystem.

## 9. Governance

The **CyberTOMP® Steering Committee** coordinates:

- The evolution of the CyberTOMP® model.  
- Ecosystem-wide releases.  
- Synchronization of participating repositories.  
- Publication of release documentation.  

All official releases and their corresponding changes are documented on the CyberTOMP® project portal.
  
