# Release Pipeline

## What is a Release Pipeline?
A release pipeline is a process that takes artifacts (such as build outputs or source code) and deploys them through multiple stages (e.g., Dev, QA, Production) until they reach production.

## Key Components of a Release Pipeline

### Artifacts
The files or packages to be deployed, typically coming from a build pipeline or source control.

### Triggers
Define what starts the release process:
- **Manual**: Started by a person.
- **Scheduled**: Runs at a specific time.
- **Continuous Deployment**: Triggered by a completed build.

### Stages/Environments
Define where the artifact is deployed, such as:
- **Development (Dev)**
- **Quality Assurance (QA)**
- **Production**

### Approvals
Can be manual or automatic checks required before moving to the next stage.

### Tasks
Steps executed in each stage to:
- Install
- Configure
- Validate the artifact

## Release vs. Release Pipeline
- **Release**: The actual deployment of an artifact.
- **Release Pipeline**: The blueprint or process used to create and manage releases.

## Key Points to Remember
- Artifacts are deployed through different stages (Dev → QA → Production).
- Triggers can be manual, scheduled, or automatic.
- Stages, approvals, and tasks are essential components.
- **Release Pipeline** = Process; **Release** = Actual deployment.

