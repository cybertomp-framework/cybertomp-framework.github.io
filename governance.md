---
layout: page
title: Governance model
subtitle: Principles, Structure, and Best Practices
cover-img:
  - "/assets/img/section-cover.png"
---

CyberTOMP® is an open framework **primarily designed to serve public sector entities**, addressing their unique challenges such as a high dependency on third-party service providers, limited agility in adopting changes, and the complexity of managing large supply chains. While its principles and practices are optimized for governmental and public service organizations, the framework remains adaptable and can also be applied in private sector contexts where similar governance challenges exist.

***

## 1. **Purpose**

The purpose of this section is to define how the CyberTOMP® Framework evolves within an open and collaborative community. Rather than governing adoption, this governance model focuses on guiding the **continuous improvement of a framework tailored to public sector realities**, while remaining flexible for broader use. It ensures that changes are transparent, inclusive, and aligned with the framework’s core principles.

## 2. **Governance Principles**

The evolution of CyberTOMP® is guided by a set of principles that reflect the spirit of openness, collaboration, usefulness and robustness:

*   **Transparency**: All decisions, discussions, and changes are documented and accessible to the community.
*   **Inclusivity**: Every member of the community has the opportunity to contribute ideas and feedback.
*   **Neutrality**: Decisions are made in the interest of the framework and its users, avoiding favoritism or commercial bias.
*   **Continuous Improvement**: The framework should adapt to emerging needs, technologies, cyberthreats and best practices without losing its foundational values.
*   **Evidence-Based Evolution**: Changes to the framework must be supported by empirical evidence, such as documented research, pilot projects, or credible third-party studies, rather than unverified personal opinions.
*   **Broad Applicability**: Enhancements should provide value to a wide range of organizations and contexts, avoiding highly specific or niche improvements that benefit only a limited set of use cases.
*   **Public Sector Priority**: The framework’s evolution should prioritize the needs of public sector entities. Private sector considerations are welcome only if they do not compromise essential public requirements.

## 3. **Scope**

This governance model applies to:

*   The process for proposing, reviewing, and approving changes to the whole framework and all its subprojects.
*   The roles and responsibilities of individuals and groups involved in its evolution.
*   Mechanisms for resolving disagreements and maintaining community harmony.

It does **not** govern:

*   How organizations implement or adopt CyberTOMP®.
*   Specific technical deployments or proprietary/derivative adaptations.
*   Actions required to grant third parties permissions to use the CyberTOMP® trademark and associated logo, as defined in the [Trademark](/trademark) section.

## 4. **Governance Structure**

The governance model is built around collaborative roles:

*   **Steering committee**: A group responsible for reviewing proposals, ensuring alignment with principles, and guiding strategic direction. The Steering Committee will be a collegial body composed of members of the GITACA research group, as the initial promoters of the project. However, this does not preclude the possibility that, in the medium term, other individuals may join if, in the judgment of the Steering Committee itself, they have demonstrated an exceptional commitment to the project and its objectives
*   **Open Community**: Contributors who share ideas, provide feedback, and participate in discussions and voting. The community members are welcome to submit their work for consideration as part of the CyberTOMP® Framework, provided it aligns with the overall governance model and adheres to the guidelines set forth in the [Contributions](/contributions) section.
*   **Facilitators**: Individuals who moderate conversations, manage collaborative platforms, and ensure smooth communication. Facilitators will be appointed from among community members by the Steering Committee, provided they have demonstrated a strong commitment to the principles outlined in the [Code of Conduct](/codeofconduct).

![Governance structure](/assets/img/governance-structure.jpg){: .mx-auto.d-block :}

## 5. **Evolution Process**

The process for evolving CyberTOMP® is designed to be open and structured:

1.  **Proposal Submission**: Any community member can submit a change proposal through the official repository following the guidelines set forth in the [Contributions](/contributions) section.
2.  **Review Phase**: The Steering Committee evaluates the proposal for technical soundness and alignment with principles, while opening it for public comments if necessary.
3.  **Approval and Voting**: Relevant decisions are made through a transparent vote by the members of the Steering Committee, taking into account compliance with the principles outlined in this governance model and, where applicable, the feedback provided by the broader community. Each decision will be communicated along with the rationale behind it. Minor changes may be approved directly if they meet the requirements established in this governance model.
4.  **Publication**: Approved changes are documented and integrated into the official framework (model, guides, materials, software...), with version notes and rationale.

## 6. **Community Participation**

Participation is the cornerstone of this governance model. Members can engage through:

*   Public forums and discussion channels.
*   Periodic surveys and voting sessions whenever needed.
*   Collaborative documentation and feedback loops.

## 7. **Version Management**

To maintain clarity and stability:

*   All projects belonging to the **CyberTOMP®** framework must be named using the format cybertomp-project_name. For example: cybertomp-framework-core, cybertomp-fleco, or cybertomp-fleco-studio
*   The cybertomp-framework-core project represents the **CyberTOMP®** framework itself. It is the main project, and all other subprojects must align with it.
*   The cybertomp-framework-core project will follow the pattern “-version”, and therefore will not include a revision number. Whenever major changes or enhancements are required that would break compatibility or alignment between the model and the rest of the projects, a new version must be released. For example, moving from **CyberTOMP®** version 1 to **CyberTOMP®** version 2 would require an evolution from cybertomp-framework-core-1 to cybertomp-framework-core-2. It is expected that the model itself will remain more stable than the rest of the projects.
*   All other projects must be versioned following the pattern “-version.revision”, where version corresponds to the version number of the overall **CyberTOMP®** framework with which the project is aligned (the version of cybertomp-framework-core project). The revision is an incremental number representing subsequent bug fixes or enhancements that remain fully compatible with the same **CyberTOMP®** framework version (the version of cybertomp-framework-core project). For example, cybertomp-fleco-studio-1.4 and cybertomp-fleco-1.0 both correspond to version 1.0 of the **CyberTOMP® framework** (cybertomp-framework-core-1), whereas cybertomp-framework-core-2.5 would correspond to version 2.0 of **CyberTOMP®** (cybertomp-framework-core-2).
*   The version of the cybertomp-framework-core project will determine the official version of the **CyberTOMP® model**. For example:
    *   **CyberTOMP®** version 1 ⇔ cybertomp-framework-core-1.
    *   **CyberTOMP®** version 2 ⇔ cybertomp-framework-core-3.
    *   **CyberTOMP®** version 3 ⇔ cybertomp-framework-core-3.
*   All projects belonging to the **CyberTOMP®** framework must be consistent with the model version they share, always, but especially when a new version of the overall framework is released. At that time, all subprojects will be tagged and released as project-version-0, indicating that they are part of a new **CyberTOMP®** framework version. Releasing a new version of cybertomp-framework-core will not be allowed unless all other projects are updated to this version simultaneously.
*   Each project repository will contain at least *master*, *dev-next* and *dev-current* branches. The *master* branch will have minimal activity and will primarily represent the latest stable release of the project. The *dev-next* branch will include all new bug fixes and enhancements aimed at the next major version of the **CyberTOMP®** framework. The *dev-current* branch will include bug-fixing and minor changes aimed to release new revisions of the current **CyberTOMP®** framework, major version.
*   Other development branches may be created if needed to evolve any feature of the project, although the must be temporary and merged/deleted once finished.
*   After a new version of the **CyberTOMP®** framework is released, previous versions will no longer evolve. They will remain unchanged and freezed for reference, use, and download, but will not accept contributions or corrections.
*   The Steering Committee will coordinate the joint release process across all subprojects, ensuring their update, stabilization, and collective readiness as a new version of the **CyberTOMP®** framework.
*   Backward compatibility is considered whenever feasible.
*   All releases, along with their corresponding major changes and additions, will be publicly documented in the [Releases](/releases) section.

## 8. **Conflict Resolution**

Disagreements are addressed through:

*   Mediation by facilitators.
*   Escalation to the Steering Committee if consensus cannot be reached.

## 9. **Transparency and Accountability**

Every decision or change will be documented in each repository using the standard tools provided by GitHub, allowing any community member to generate and review the corresponding changelog.

## 10. **Licensing and Intellectual Property**

CyberTOMP® operates under open licenses that guarantee free access and contribution. Contributors are acknowledged for their work, fostering a culture of recognition and respect. However, to ensure proper management of contributions and to prevent future licensing issues with content, materials, or software, each contributor must accept a **Contribution License Agreement**, as described in the [Contributions](/contributions) section.The contributor’s acceptance of this CLA does not imply that the proposed contribution will be accepted, which will require the approvals and validations described in this governance model.

