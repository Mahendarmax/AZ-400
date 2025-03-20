# Set Up and Run Availability Tests

## Overview
This document explains how to set up and run availability tests to monitor the health and responsiveness of web applications or websites.

## Key Concepts

### 1. Purpose of Availability Tests
- Monitor the availability and responsiveness of web apps or websites.
- Ensure the application is running and providing healthy responses.

### 2. Health Endpoints
- Specific endpoints can be created to check application health.
- Examples: HTTP status checks or complex computations involving critical components (e.g., database queries).

### 3. Availability Test Frameworks
- Custom frameworks can be created for ping tests.
- Platforms like Azure provide built-in functionality for availability tests.

### 4. Azure Availability Tests
- Can be used in pipelines and as release gates.
- Supports HTTP/HTTPS endpoints accessible from the public internet.
- No additional setup is required on the website being tested.

### 5. Types of Availability Tests in Azure
#### URL Ping Test
- Simple test created in the Azure portal.
- Checks URL response and status code.

#### Multi-Step Web Test
- Executes a sequence of HTTP calls.
- Useful for testing complex workflows.

### 6. Use Cases
- Monitor your own web applications or REST APIs.
- Test third-party services your application depends on.

## Summary
- Availability tests are essential for monitoring application health and responsiveness.
- Use Azure's built-in tools for URL ping tests and multi-step web tests.
- Health endpoints can provide deeper insights into application functionality.