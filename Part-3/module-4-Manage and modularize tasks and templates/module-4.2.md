# Variables in Release Pipelines

## Overview
Variables in release pipelines provide a convenient way to pass critical data into various parts of the pipeline. They can change between releases, stages, or jobs and are essential for configuring and customizing pipeline behavior.

---

## Key Concepts

### Purpose of Variables
- Store and pass critical data (e.g., server names, connection strings, passwords).
- Values can change between releases, stages, or jobs.

### Variable Scope
Variables can have different scopes:
- **Release Pipeline:** Available across all stages and tasks.
- **Stage:** Available only within a specific stage.
- **Task:** Available only within a specific task.

### Types of Variables
- **Predefined Variables:** Automatically provided by the system (e.g., agent directory, build number, agent name).
- **Custom Variables:** Defined by the user for specific needs.
- **Secret Variables:** Hidden from logs and used for sensitive data (e.g., passwords).

---

## Predefined Variables
System-provided variables that are always available during a release pipeline run.

### Examples:
- `Build.BuildNumber`: The build number of the release.
- `Agent.Name`: The name of the agent running the pipeline.
- `Release.EnvironmentName`: The name of the current stage/environment.

---

## Variable Scopes and Use Cases

### Release Pipeline Variables
- **Scope:** Available across all stages and tasks in the release pipeline.
- **Use Case:** Use when you need the same value across all stages and want to change it in one place.
- **Example:** A variable like `TargetServer` can be used across multiple stages.

### Stage Variables
- **Scope:** Available only within a specific stage.
- **Use Case:** Use when values vary between stages but are the same for all tasks within a stage.
- **Example:** A variable like `DatabaseConnectionString` can have different values for Dev and Test stages.

### Variable Groups
- **Scope:** Shared across all pipelines and stages in a project.
- **Use Case:** Use when you need to share values across multiple pipelines.
- **Example:** Store common configuration values like API keys or environment URLs.

---

## Normal vs. Secret Variables
| Feature        | Normal Variables | Secret Variables |
|---------------|----------------|----------------|
| **Visibility** | Visible in logs and outputs | Hidden from logs |
| **Use Case**   | Non-sensitive data (e.g., URLs) | Sensitive data (e.g., passwords) |
| **Security**   | Exposed as clear text | Encrypted and masked in logs |

---

## Best Practices
- **Use Descriptive Names:** Name variables clearly (e.g., `Prod_DB_ConnectionString`).
- **Scope Appropriately:** Use the smallest scope necessary (e.g., stage-level for stage-specific values).
- **Use Secret Variables for Sensitive Data:** Always mark passwords, API keys, and other sensitive data as secret.
- **Leverage Variable Groups:** Use variable groups to share values across multiple pipelines.

---

## Exam Tips

### Key Concepts:
- Understand the purpose and scope of variables.
- Know the difference between predefined, custom, and secret variables.
- Be familiar with variable groups and their use cases.

### Scenario-Based Questions:
Be prepared for questions like:
- "How can you securely store a password in a release pipeline?"
- "What is the scope of a stage-level variable?"

### Key Terminology:
- **Predefined variables**
- **Secret variables**
- **Variable groups**
- **Scope**

---

## References
- **[Release Variables and Debugging](https://learn.microsoft.com/en-us/azure/devops/pipelines/release/variables?view=azure-devops)**
- **[Variable Groups](https://learn.microsoft.com/en-us/azure/devops/pipelines/library/variable-groups?view=azure-devops)**