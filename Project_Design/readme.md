# Laptop Request Catalog - Project Design Phase

* *Project Name:* LAPTOP REQUEST CATALOG ITEM
* *Team ID:* NM2025TMID04453
* *Date:* 02 NOVEMBER 2025

---

## 1. Problem-Solution Fit

This phase defines the direct relationship between the user's problem and the solution we are building.

### Problem
University staff and students face significant difficulties in requesting laptops. The current manual, email-based processes cause delays, lack transparency, and lead to frequent miscommunication. There is no centralized system, resulting in approval bottlenecks, duplicate requests, and inefficient asset tracking.

### Solution
A digital ServiceNow-based Laptop Request Catalog Item provides a structured, automated workflow. This solution simplifies the process with an easy-to-use online form, reduces approval delays, and ensures full transparency in request tracking.

### Purpose of the Solution
* To provide an easy and efficient way for users to request laptops through an online system.
* To streamline the approval and allocation process for academic or work-related needs.
* To reduce manual paperwork and processing delays.
* To enhance transparency by allowing users to track the status of their requests.
* To ensure proper resource management and timely laptop distribution.

---

## 2. Proposed Solution

The proposed solution is a comprehensive *Laptop Request Catalog Item* built on the ServiceNow platform. This system will digitize the entire request lifecycle, from initial submission to final delivery and asset tracking.

The solution is designed to address the specific pains of both students and administrators:
* *For Students (Requesters):* A streamlined digital request form where they can submit, track, and receive automatic updates. This eliminates the frustration and uncertainty of manual processes.
* *For IT Administrators:* An automated approval workflow with central visibility. This prevents lost requests, ensures traceability, and enables faster, more accurate laptop allocation.

*Key features identified during brainstorming include:*
* A user-friendly catalog form with fields for model, justification, and required date.
* An automated manager approval workflow that triggers before the request is submitted for fulfillment.
* Dynamic model selection based on current availability.
* Automated email notifications for each approval stage to keep all stakeholders informed.

---

## 3. Solution Architecture

The solution is architected as a complete, end-to-end process within ServiceNow. The design and deployment process follows these key steps:

1.  *Design the Laptop Needs (Form):* Create the user-facing catalog item form in ServiceNow.
2.  *Identify Laptops (Catalog):* Define the available laptop models that users can request.
3.  *Configure the Approval Workflow:* Build the automated, hierarchical approval workflow (e.g., for manager approval).
4.  *Configure Workflow (Fulfillment):* Create the fulfillment tasks for the IT team that trigger after approval.
5.  *Integrate with CMDB:* Connect the workflow to the Configuration Management Database (CMDB) for accurate asset tracking and management.
6.  *Automate Notifications:* Configure email and portal notifications for users and approvers at key stages.
7.  *Test and Validate Process:* Thoroughly test the entire flow, from submission to approval and task generation.
8.  *Deploy and Monitor Requests:* Make the catalog item available to users and monitor its performance.