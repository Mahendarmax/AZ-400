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

## What is an Artifact?
A deployable component of your application (e.g., a package, file, or container image).

Used in build and release pipelines for Continuous Delivery.

### Key Principle
**Build once, deploy many times**: The artifact should be immutable (unchanged) across environments. Only configurations change for different environments.

## Common Artifact Sources

### Build Artifacts
- Created by a build pipeline (compiled, tested, and versioned).
- Stored securely (e.g., storage account, database).
- Provides traceability (linked to the build).

### Version Control
- Directly linked to a specific commit in version control (e.g., Git).
- Useful for deploying single files or helper scripts (e.g., cleanup scripts).

### Network Share
- Files stored on a shared network location.
- Risky because files can be changed or compromised by others.
- Not suitable for regulated environments (e.g., banks, insurance).

### Container Registries
- Versioned repositories for container images (e.g., Docker images).
- Secure and traceable, similar to build artifacts.

## Key Considerations
- Use build artifacts for versioned, immutable packages.
- Use version control for specific files or scripts.
- Avoid network shares in regulated environments due to integrity risks.
- Use container registries for containerized applications.

## Key Points to Remember
- Artifacts are deployable components.
- Immutability ensures the artifact doesn’t change after creation.
- Common sources: Build artifacts, version control, network shares, container registries.
- Build artifacts and container registries are secure and versioned.
- Network shares are risky for regulated environments.

## Key Points to Remember
- Artifacts are deployed through different stages (Dev → QA → Production).
- Triggers can be manual, scheduled, or automatic.
- Stages, approvals, and tasks are essential components.
- **Release Pipeline** = Process; **Release** = Actual deployment.

