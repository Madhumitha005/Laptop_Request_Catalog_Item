# Laptop Request Catalog - Requirement Analysis

* *Project Name:* LAPTOP REQUEST CATALOG ITEM
* *Team ID:* NM2025TMID04453
* *Date:* 02 November 2025

---

## 1. Solution Requirements

Based on the Ideation and Design phases, the following functional and non-functional requirements were defined to solve the identified user problems.

### High-Level Goals
The primary purpose of the solution is to:
* Provide an easy and efficient way for users to request laptops through an online system.
* Streamline the approval and allocation process for academic or work-related needs.
* Reduce manual paperwork and processing delays.
* Enhance transparency by allowing users to track the status of their requests.
* Ensure proper resource management and timely laptop distribution.

### Functional Requirements
To achieve these goals, the system must include the following features:

* *Digital Request Form:* A centralized, digital catalog item in ServiceNow to replace manual forms and email submissions.
* *Automated Approval Workflow:* An automated, hierarchical approval workflow to route requests to the correct manager, reducing bottlenecks and manual intervention.
* *Real-time Request Tracking:* A user-facing portal where users can see the status and progress of their laptop requests in real-time.
* *Automated Notifications:* Integrate email and portal notifications to alert users and approvers at each stage of the request (submission, approval, fulfillment, closure).
* *CMDB Integration:* The catalog workflow must integrate with the CMDB (Configuration Management Database) for accurate asset tracking, management, and assignment.
* *Validation Rules:* The system must implement validation to prevent duplicate or identical requests from being submitted.
* *Dynamic Fields:* The catalog form should include dynamic fields, such as model selection based on current availability.

---

## 2. Data Flow Diagram

The following describes the flow of data through the "Laptop Request" system, from submission to fulfillment.

1.  *Submission:* The *User (Student/Staff)* accesses the Service Portal and inputs request data (e.g., justification, laptop type) into the *Laptop Request Catalog Form*.
2.  *Approval:* Upon submission, the request data is routed to the *Approval Workflow. The system sends a notification and approval request (data) to the user's **Manager*.
3.  *Fulfillment:* Once the manager approves, the request data is passed to the *Fulfillment Workflow. A fulfillment task is created and assigned to the **IT Team*.
4.  *Asset Management:* The *IT Team* uses the task data to provision a laptop. The new asset information is updated in the *CMDB* and linked to the user's record.
5.  *Closure:* Upon task completion, the system updates the request status to "Complete." A final notification (data) is sent to the *User*, and the request data is archived for reporting.

---

## 3. Technology Stack

The solution is built entirely within the *ServiceNow* platform. The following key modules and technologies are required:

* *Core Platform:* ServiceNow
* *Service Portal:* Provides the user-facing front-end for submitting the request.
* *Service Catalog:* Used to create, define, and manage the "Laptop Request Catalog Item" and its form fields.
* *Workflow / Flow Designer:* The engine used to build the automated approval and fulfillment workflows.
* *CMDB (Configuration Management Database):* The database used for tracking and managing laptop assets and linking them to users.
* *Notification System:* Manages the automated email and portal alerts for users and approvers.