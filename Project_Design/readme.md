# Laptop Request Catalog - Project Design Phase

* *Project Name:* LAPTOP REQUEST CATALOG ITEM
* *Team ID:* NM2025TMID04453
* *Date:* 02 November 2025

---

## 1. Problem-Solution Fit

This phase defines the direct relationship between the user's problem and the designed solution.

### Problem
Users (university staff and students) face significant difficulties in requesting laptops for academic or administrative purposes. The current manual or email-based processes cause delays, lack transparency, and lead to frequent miscommunication. There is no centralized system, resulting in approval bottlenecks, duplicate requests, and inefficient asset tracking.

### Solution
A digital ServiceNow-based Laptop Request Catalog Item provides a structured, automated workflow. This solution simplifies the process with an easy-to-use online form, reduces approval delays, and ensures full transparency in request tracking. The system effectively meets user needs by connecting them with the right IT resources.

### Purpose of the Solution
* To provide an easy and efficient way for users to request laptops through an online system.
* To streamline the approval and allocation process for academic or work-related needs.
* To reduce manual paperwork and processing delays.
* To enhance transparency by allowing users to track the status of their requests.
* To ensure proper resource management and timely laptop distribution.

---

## 2. Proposed Solution

Based on the problems identified, the team agreed to create a streamlined laptop request catalog item with automated approvals. The proposed solution is a digital catalog form in ServiceNow that automates submissions and approvals.

Key features of the proposed solution include:
* *Digital Catalog Form:* Create a catalog item in ServiceNow with fields for model, justification, and required date.
* *Automated Approvals:* Add a manager approval workflow that triggers before the request is submitted for fulfillment. This reduces manual intervention.
* *Dynamic Content:* Include dynamic model selection based on current availability.
* *Notifications:* Integrate email notifications for each approval stage to keep users and approvers informed.
* *Validation:* Implement validation rules to prevent duplicate requests and ensure all required details are submitted.

---

## 3. Solution Architecture

The solution is architected as an end-to-end design and deployment process within ServiceNow. The high-level architecture follows these steps:

1.  *Design the Laptop Needs:* Define and design the user-facing catalog request form.
2.  *Identify Laptops:* Specify the laptop models and details available to be requested.
3.  *Configure the Approval Workflow:* Build the automated, hierarchical approval workflow (e.g., manager approval).
4.  *Configure Workflow (Fulfillment):* Create the automated fulfillment workflow that generates tasks for the IT team post-approval.
5.  *Integrate with CMDB:* Connect the workflow to the Configuration Management Database (CMDB) for accurate asset tracking and management.
6.  *Automate Notifications:* Configure automated email and portal notifications for all stakeholders.
7.  *Test and Validate Process:* Thoroughly test the end-to-end process to ensure all components function correctly.
8.  *Deploy and Monitor Requests:* Deploy the catalog item to the production environment and monitor incoming requests.