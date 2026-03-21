# **Evidence Index CSV Guide (V5)**

This document defines the schema and data types for the evidence\_index.csv file, which serves as the canonical record linking deployable artifacts (files) to their corresponding task tickets and project blueprints.

This V5 schema update formalizes the use of the 8-column structure and includes explicit guidelines for the **Three-Way Audit Traceability** model.

## **Required Schema Fields (8 Columns)**

The index file **must** contain the following eight (8) columns in this exact order.

| Column Name | Type | Description | Example Value |
| :---- | :---- | :---- | :---- |
| **PROJECT\_PREFIX** | String | A short, unique identifier for the project this evidence belongs to (e.g., used as the prefix on tickets). | API or WEB |
| **MOD\_CODE** | String | **(Critical Link)** The Internal Module Code (e.g., MOD\_FTM\_001) that defines the design specifications this evidence supports. | MOD\_RCM\_001 |
| **TICKET** | String | The unique task identifier associated with the work (e.g., the specific CRUD operation). | WP1.2.3.4 |
| **EVIDENCE\_ID** | UUID/String | A unique, non-sequential identifier for this specific piece of evidence. Used to prevent duplicates. | d2f4a9b0-8c2e-4b71-93e1-2a1f8c7b6d5e |
| **FILE\_NAME** | String | The complete file name, including its extension, as deployed in the asset bucket. | compliance\_audit\_v2.pdf |
| **FILE\_HASH** | String | The SHA-256 hash of the file content. Used to verify file integrity post-deployment. | a0b1c2d3e4f5a0b1c2d3e4f5a0b1c2d3e4f5a0b1c2d3e4f5a0b1c2d3e4f5a0b1 |
| **TIMESTAMP** | ISO 8601 | The UTC timestamp when the file was indexed and deployed. | 2025-10-23T17:55:00Z |
| **DESCRIPTION** | String | A brief, plain-language description of the file's contents or purpose. | Screenshot confirming TPT fine is applied. |

## **Rationale: The Three-Way Audit Traceability**

For any project artifact, especially in a regulated environment, auditors need to trace the "proof" back to the "design." The evidence\_index.csv achieves this using three key fields:

| Field | Purpose for Volunteers | Example (Compliance Check) |
| :---- | :---- | :---- |
| **MOD\_CODE** | **The Design (Blueprint):** What *module* or *specification* required this work? (The **WHY** of the task). | MOD\_RCM\_001 (Reputation & Curation Module) |
| **TICKET** | **The Task (Work Item):** What *specific action* did you perform? (The **HOW** it was done). | RCM-107 (Task: Implement TPT debt creation endpoint.) |
| **Evidence File** | **The Proof:** What *file* shows the work item was completed correctly? (The **PROOF** it works). | tpt\_debt\_unit\_test.log |

**Rule for Interns/Volunteers:**

1. Always look up the **MOD\_CODE** first. This tells you which SSDD document (e.g., MOD\_FTM\_001.md) defines the rule you are proving.  
2. Then, use the **TICKET** to find the specific task you just finished.  
3. Fill in the rest of the file metadata. The MOD\_CODE and TICKET must **always** be filled out before indexing evidence.
