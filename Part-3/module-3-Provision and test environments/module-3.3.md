# Understand Shift-Left

## Overview
This document explains the concept of Shift-Left in software development, focusing on moving testing earlier in the pipeline to improve quality and reduce failures.

## Key Concepts

### 1. Goal of Shift-Left
- Move quality upstream by performing tests early in the pipeline.
- Encourages "fail fast, fail often" to reduce the impact of failures later.

### 2. Importance of Early Testing
- Ensures most testing is complete before merging changes into the main branch.
- Prevents delays caused by long-running tests later in the development lifecycle.

### 3. Challenges with Scaling Tests
- As projects grow, the number and complexity of tests increase.
- Long-running tests (hours or days) are often delayed, reducing their effectiveness.

### 4. Principles for DevOps Teams
- Focus on fast and reliable unit tests.
- Ensure functional tests are independent.
- Define a clear test taxonomy for different scenarios.

### 5. Test Taxonomy
#### L0 Tests
- Fast in-memory unit tests dependent only on the code in the assembly under test.

#### L1 Tests
- Require assembly plus external dependencies like SQL or the file system.

#### L2 Tests
- Functional tests run against testable service deployments with critical dependencies stubbed out.

#### L3 Tests
- Integration tests run against production, requiring a complete product deployment.

### 6. Case Study
- Microsoft runs over 60,000 unit tests in parallel in less than 6 minutes, aiming to reduce this to under a minute.

### 7. Shift-Right Testing
- Testing in production to validate real-world scenarios.

## Summary
- Shift-Left emphasizes early testing to improve quality and reduce failures.
- Define a clear test taxonomy and focus on fast, reliable tests.
- Use Shift-Right testing to validate production scenarios.



