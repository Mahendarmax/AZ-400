# Release Approvals

This document explores the concept of **release approvals** in the context of Continuous Delivery (CD) and their importance in the release management process.

---

## **Overview**
- **Continuous Delivery (CD)**: Focuses on delivering software on-demand.
- **Release vs. Deployment**: Deployment is the technical process of installing software, while release approvals control **if** the software should be delivered.
- **Purpose of Approvals**: To ensure compliance, manage dependencies, and maintain control over the release process.

---

## **Key Concepts**

### **Manual Approvals**
- **Initial Need**: Organizations new to CD often lack trust in automated processes and rely on manual approvals.
- **Evolution**: Over time, if releases consistently succeed, manual approvals may be replaced by automated checks.
- **Use Cases**:
  - Compliance requirements (e.g., SOX compliance, four-eyes principle).
  - Dependency management.
  - Sign-off from authorities (e.g., Security Officers, Product Owners).

### **Automatic Approvals (Release Gates)**
- **Purpose**: To eliminate manual intervention while maintaining control over the release process.
- **Example**: Automated checks can be performed earlier in the pipeline (e.g., approving changes in Source Control).
- **Benefits**: Reduces delays and ensures consistency.

---

## **Things to Consider When Setting Up Release Approvals**

### 1. **What Do We Want to Achieve?**
   - Is the approval needed for **compliance** (e.g., SOX, four-eyes principle)?
   - Is it for **dependency management**?
   - Is it for **authority sign-off** (e.g., Security Officers, Product Owners)?

### 2. **Who Needs to Approve?**
   - Identify the approver(s): Product Owner, Security Officer, or someone independent of the development team.
   - Consider availability: Approvers can delay the process if they are unavailable.

### 3. **When to Approve?**
   - Timing is critical: Approval can be separated from deployment using **scheduled deployments**.
   - Decide if the process can continue without approval or if everything is on hold until approval is given.

---

## **Scheduled Deployments**
- **Purpose**: Separates approval from deployment to avoid delays.
- **Example**: Deployments can be scheduled for specific times (e.g., nightly), reducing the need for manual intervention during off-hours.

---

## **When Manual Approvals Are Not Helpful**
- **Early Checks**: Manual approvals can sometimes be replaced by checks earlier in the pipeline (e.g., approving changes in Source Control).
- **Automation**: Use **automatic approvals** or **release gates** to eliminate manual activities while maintaining control.

---

## **Key Takeaways for AZ-400 Exam**
1. **Understand the Role of Approvals**:
   - Manual approvals provide control but can slow down the process.
   - Automatic approvals (release gates) streamline the process while maintaining oversight.

2. **Scenario-Based Questions**:
   - Be prepared to identify when to use manual vs. automatic approvals.
   - Understand the trade-offs between compliance, control, and speed.

3. **Integration with Release Pipelines**:
   - Approvals are a critical part of the release pipeline and influence the delivery cadence.

---