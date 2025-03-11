# Delivery Cadence and Triggers

This document provides an overview of delivery cadence and the three types of triggers used in release pipelines, particularly from an **AZ-400 exam** perspective.

---

## **Delivery Cadence**
- **Definition**: The frequency and consistency with which software releases are deployed to production or other environments.
- **Importance**: Ensures a predictable and efficient release process, enabling faster delivery of value to end-users.
- **Key Factors**: Influenced by the type of triggers used in the release pipeline.

---

## **Three Types of Triggers**

### 1. Continuous Deployment Trigger
- Automatically triggers a release pipeline when a new build is completed.
- Ensures that every successful build results in a new release.
- Ideal for teams practicing **Continuous Integration (CI)** and **Continuous Deployment (CD)**.
- **Example**: A new build is created, and the release pipeline automatically deploys it to the target environment.

### 2. Scheduled Trigger
- Allows releases to be triggered at a specific time or interval.
- Useful for scenarios where releases need to occur at predictable times (e.g., nightly builds or scheduled deployments).
- Can be configured for multiple schedules (e.g., daily at 3:00 AM or 12:00 PM).
- **Example**: A release pipeline is configured to deploy updates every night at 2:00 AM.

### 3. Manual Trigger
- Requires human intervention or an external system to initiate the release.
- Used when releases need to be approved or triggered based on specific events.
- Can be initiated via a UI (by a person) or through an automation engine (by a system).
- **Example**: A team lead manually approves and triggers a release after reviewing the build.

---

## **Key Points for AZ-400 Exam**
1. **Understand the Use Cases**:
   - **Continuous Deployment Trigger**: Best for fully automated CI/CD pipelines.
   - **Scheduled Trigger**: Ideal for time-based releases (e.g., nightly builds).
   - **Manual Trigger**: Used when human approval or external events are required.

2. **Integration with Release Pipelines**:
   - Triggers are configured within the release pipeline to control when and how releases are deployed.

3. **Automation and Flexibility**:
   - Continuous Deployment and Scheduled Triggers emphasize automation.
   - Manual Triggers provide flexibility for controlled releases.

4. **Scenario-Based Questions**:
   - Be prepared to identify the appropriate trigger type based on a given scenario (e.g., automated vs. manual releases).

---