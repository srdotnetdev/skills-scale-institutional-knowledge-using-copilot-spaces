# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA/Test Engineer

### Role Summary
QA/Test Engineers own test strategy and release-quality signals. They help the team find defects and risks early and confirm that work meets acceptance criteria before release.

### Responsibilities
- Define test strategy, test plans, and regression suites
- Validate features against acceptance criteria
- Triage defects and report quality risks
- Provide release-readiness sign-off input

### Decision Rights / Ownership Boundaries
- Owns: test plans, defect reports, release quality report
- Decides: test scope and whether quality criteria are met (can raise a release-blocking concern)
- Does not decide: product scope or release dates

### Key Artifacts Owned or Co-owned
- Test plans and regression suites (owned)
- Defect log and quality dashboard (owned)
- Acceptance criteria (co-owned with Product Managers)
- Release checklist (co-owned with DevOps)

### Typical Communication Cadence
- Participates in daily standups and sprint planning
- Weekly quality summary to Project Managers
- Defect triage and release-readiness reviews

### Interaction Map with Existing Roles
- Developers: receive defect reports and fixes; agree on unit vs. integration test boundaries
- Product Managers: clarify acceptance criteria and accept test outcomes
- Project Managers: escalate quality risks and report test status for the risk register

---

## UX/UI Designer

### Role Summary
UX/UI Designers shape the user experience and interface. They turn user needs and product goals into designs the team can build and validate.

### Responsibilities
- Conduct user research and usability testing with Product Managers
- Produce wireframes, prototypes, and design specs
- Maintain the design system and accessibility standards
- Review implemented UI against designs

### Decision Rights / Ownership Boundaries
- Owns: interaction design, visual design, and design system standards
- Decides: UI patterns and accessibility approach within product goals
- Does not decide: product priorities or technical architecture

### Key Artifacts Owned or Co-owned
- Wireframes, prototypes, and design specs (owned)
- Design system (owned)
- Usability findings (co-owned with Product Managers)
- Acceptance criteria for UI behavior (co-owned with Product Managers and QA)

### Typical Communication Cadence
- Weekly design reviews with Product Managers
- Design handoff sessions before sprint planning
- Async feedback on PRs and design comments

### Interaction Map with Existing Roles
- Developers: handoff designs, answer implementation questions, review UI
- Product Managers: align on user problems, research, and priorities
- Project Managers: share design timelines and dependencies for planning

---

## DevOps / Platform Engineer

### Role Summary
DevOps / Platform Engineers build and operate the pipelines, environments, and infrastructure that make delivery repeatable, reliable, and observable.

### Responsibilities
- Maintain CI/CD pipelines and environments
- Automate deployments, rollbacks, and infrastructure as code
- Monitor reliability, performance, and cost
- Support incident response and post-incident reviews

### Decision Rights / Ownership Boundaries
- Owns: pipelines, environments, deployment tooling, and monitoring
- Decides: infrastructure and deployment mechanics; can pause a deployment for reliability reasons
- Does not decide: feature scope or release business timing

### Key Artifacts Owned or Co-owned
- CI/CD pipeline and infrastructure code (owned)
- Runbooks and monitoring dashboards (owned)
- Release and rollback plan (co-owned with Project Managers)
- Release checklist (co-owned with QA)

### Typical Communication Cadence
- Daily standups during release windows
- Release planning and deployment coordination
- Incident updates and post-incident reviews

### Interaction Map with Existing Roles
- Developers: provide pipelines, environments, and deployment guidance; developers supply deployable, observable code
- Product Managers: communicate release capabilities and constraints
- Project Managers: coordinate release windows, dependencies, and incident communication

---

## Security / Compliance Lead

### Role Summary
Security / Compliance Leads protect the product and organization by defining security and regulatory requirements and verifying they are met throughout delivery.

### Responsibilities
- Define security and compliance requirements
- Perform threat modeling and risk assessments
- Review designs, dependencies, and releases for security impact
- Track vulnerabilities and remediation

### Decision Rights / Ownership Boundaries
- Owns: security policies, compliance requirements, and risk acceptance recommendations
- Decides: whether security/compliance gates are met; can block a release with documented rationale
- Does not decide: product priorities beyond compliance obligations

### Key Artifacts Owned or Co-owned
- Security requirements and threat models (owned)
- Vulnerability and compliance tracker (owned)
- Risk register entries for security (co-owned with Project Managers)
- Release security sign-off (co-owned with DevOps)

### Typical Communication Cadence
- Security review at design and pre-release milestones
- Monthly compliance and vulnerability summary
- Ad hoc escalation for critical findings

### Interaction Map with Existing Roles
- Developers: provide secure coding guidance and review findings; developers remediate issues
- Product Managers: advise on compliance impact of features and trade-offs
- Project Managers: contribute to risk register and schedule reviews early

---

## Data Analyst / Insights Partner

### Role Summary
Data Analysts / Insights Partners turn product and delivery data into insights that inform prioritization, measure outcomes, and improve processes.

### Responsibilities
- Define metrics and instrumentation requirements with Product Managers
- Build dashboards and analyses of product and delivery data
- Measure outcomes against success metrics
- Share insights for retrospectives and planning

### Decision Rights / Ownership Boundaries
- Owns: metric definitions, analyses, and dashboards
- Decides: analytical methods and data quality standards
- Does not decide: priorities or how to act on insights

### Key Artifacts Owned or Co-owned
- Metrics definitions and dashboards (owned)
- Success metrics (co-owned with Product Managers)
- Delivery metrics reports (co-owned with Project Managers)
- Instrumentation requirements (co-owned with Developers)

### Typical Communication Cadence
- Bi-weekly insights review with Product Managers
- Input to retrospectives and quarterly planning
- Ad hoc analysis requests

### Interaction Map with Existing Roles
- Developers: specify instrumentation and data needs; developers implement tracking
- Product Managers: partner on success metrics and outcome measurement
- Project Managers: provide delivery metrics such as cycle time and risk trends

---

## Customer Support / Enablement Representative

### Role Summary
Customer Support / Enablement Representatives are the voice of the customer after release. They support onboarding, resolve issues, and prepare customers and internal teams for change.

### Responsibilities
- Triage and resolve customer issues and feed patterns back to the team
- Prepare enablement materials and training for new releases
- Support customer onboarding
- Provide customer feedback for prioritization

### Decision Rights / Ownership Boundaries
- Owns: support processes, customer escalations, and enablement plans
- Decides: support handling and escalation paths
- Does not decide: fixes or roadmap priorities

### Key Artifacts Owned or Co-owned
- Support knowledge base and FAQs (owned)
- Customer issue and feedback summaries (owned)
- Release communications and enablement plan (co-owned with Product Managers and Technical Writers)
- Known issues list (co-owned with QA)

### Typical Communication Cadence
- Weekly customer feedback summary to Product Managers
- Pre-release enablement briefings
- Escalations as needed during incidents

### Interaction Map with Existing Roles
- Developers: escalate reproducible issues with context; developers provide root cause updates
- Product Managers: share customer trends and receive release notes
- Project Managers: coordinate release communications and escalation timelines

---

## Technical Writer / Documentation Owner

### Role Summary
Technical Writers / Documentation Owners keep documentation accurate, consistent, and discoverable so teams and customers can work repeatably.

### Responsibilities
- Create and maintain user, process, and technical documentation
- Define documentation standards and templates
- Review documentation updates as part of release readiness
- Support onboarding with clear guides

### Decision Rights / Ownership Boundaries
- Owns: documentation standards, structure, and publication
- Decides: style, templates, and information architecture
- Does not decide: product behavior or process policy content (owners approve their content)

### Key Artifacts Owned or Co-owned
- Documentation standards and templates (owned)
- Release notes and user guides (co-owned with Product Managers)
- Process docs (co-owned with Project Managers)
- Technical docs and READMEs (co-owned with Developers)

### Typical Communication Cadence
- Documentation review at sprint boundaries
- Release documentation checkpoints
- Async review on documentation PRs

### Interaction Map with Existing Roles
- Developers: collaborate on technical docs and API references; developers review accuracy
- Product Managers: align on release notes and user-facing content
- Project Managers: keep process docs current and consistent with status reporting

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

