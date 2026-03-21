# **VIBE CODE Policy for Upskilling Project Volunteers**

## **Audit Tracking Header**

| Field | Value |
| :---- | :---- |
| **Document ID** | **POL-20251102-038** |
| **Filepath** | **docs/policies/vibe\_code\_policy.md** |
| **Document Title** | **VIBE CODE Policy for Upskilling Project** |
| **Internal Module Code** | **MOD\_SYS\_038** |
| EU WP Code (Legacy) | N/A (Placeholder: WPX\_DXX.X) |
| **Document Revision** | **v02** |
| Date Created | **2025-11-02** |
| **Last Modified** | **2025-11-02** |
| Conceptual Author | You |
| Documenting Author | Gemini LLM |
| Module Owner (Legal) | Makea B.V. |
| Operational Owner | Hèlen Grives |
| GitHub Commit Hash | N/A (Placeholder: a1b2c3d) |
| Evidence Folder Path | N/A (Placeholder: /06\_Deliverables/...) |
| SHA256 Checksum | N/A (Only for final PDF version) |
| **Status** | **Draft** |
| Linked Budget Line | N/A (Placeholder: B.1 Personnel) |
| Related Deliverable Sheet | N/A (Placeholder: Filename/Link) |
| Notes | Policy defining rules for AI-assisted coding (Vibe Coding) and skill assessment (LeetCode) for upskilling volunteers. |

## **1\. Introduction and Purpose**

This VIBE CODE Policy ("Policy") is designed to guide volunteers participating in the upskilling project, particularly those with **weak or beginner programming skills**.

The term **"Vibe Coding"** refers to the practice of relying on AI-assisted tools (like large language models or code co-pilots) through intuition, trial-and-error, or rapid generation, often without a thorough understanding of the underlying code.

The purpose of this policy is to ensure that AI-assisted coding is used as a **learning accelerator** and not a shortcut, maintaining a critical balance between **speed, accessibility, and code quality** for all project deliverables.

## **2\. The V.I.B.E. CODE Principles**

All volunteers must adhere to the following principles when using AI-assisted tools for coding tasks:

| Principle | Description |
| :---- | :---- |
| **V**erification and Validation | **Never accept AI-generated code blindly.** Always verify the code's logic and functionality through testing and line-by-line review. You must understand *why* the code works, not just *that* it works. |
| **I**ntention-First Learning | Before prompting an AI tool, **clearly define the goal** and attempt the task using your own knowledge first. Use the AI to *check* your understanding, *debug* your existing code, or *suggest* alternatives, but never to replace the initial intellectual effort. |
| **B**est Practices & Review | Ensure AI-generated code adheres to the project's **coding standards, documentation requirements, and security practices.** Treat AI output as a draft that requires your critical, expert review and refinement. |
| **E**thical Use & Attribution | Use AI tools responsibly. Do not use them for plagiarizing existing work or generating code that violates licensing agreements. Be prepared to **document and attribute** the use of AI as required by project guidelines. |

## **2.1. Permitted and Prohibited AI Tools**

To ensure consistency, security, and compliance across the project, the use of AI-assisted coding tools is strictly limited:

* **Permitted Tools (Default):**  
  * **Gemini (Google)**  
  * **GitHub Copilot**  
  * **Microsoft Co-Pilot**  
* **Other Tools:** Use of any other AI tool requires explicit, written permission from the Project Lead.  
* **Prohibited Tools:**  
  * **OpenAI products** (including ChatGPT, GPT-4/3.5 models) are **strictly prohibited** for code generation or review within this project environment.

## **3\. Specific Guidelines for Upskilling Novice Coders**

Given the focus of this project is skill development, volunteers with weak programming skills should adhere to these additional, specific guidelines to maximize their learning:

### **3.1. Deep Dive Understanding**

For every function, class, or script you submit, you must be able to **explain its logic and every individual line of code** to a mentor or peer without relying on the AI tool. If you cannot explain it, you must spend time researching the components until you achieve full comprehension.

### **3.2. Prohibited Shortcuts**

AI tools **must not** be used to generate complete solutions for core learning assignments or challenges where the primary goal is to practice a specific concept (e.g., recursive functions, specific algorithms). The AI should only be used in these scenarios for debugging your self-written code.

### **3.3. Mandatory Quality Assurance (QA)**

The use of AI tools **does not exempt** you from rigorous testing. AI-generated code may be fast but is often flawed; your responsibility is to ensure its **reliability, efficiency, and maintainability** before submission. Implement unit tests, functional tests, or manual testing protocols as required.

### **3.4. Documentation of Assistance and Prompt Record (Updated)**

In addition to documenting AI assistance in code comments, volunteers must maintain a comprehensive record of their interactions for knowledge transfer and review:

* **Prompt Record:** A log of the prompt-response exchange (the "Prompt Record") must be kept for every significant block of generated code.  
* **Isolated Chat Documentation:** For the development of an algorithm, module, or core feature, the entire thought process—documented through subsequent prompts and refined AI outputs—must be saved in a dedicated text file (e.g., feature\_name\_prompt\_log.txt). This file should be stored alongside the relevant code, documenting the journey from initial prompt to final code.

### **3.5. Full Prototypes & Repository Storage**

When using AI to generate a complete or near-complete component, module, or application for experimentation (a "Full Prototype"), this code must be isolated and clearly marked.

* All **Full Prototypes** must be committed to the project's repository under the designated subfolder: prototypes/.  
* Prototypes should be accompanied by a brief README file explaining the AI used, the objective of the experiment, and any limitations.

### **3.6. Skill Assessment & Progress Tracking (LeetCode)**

Due to the reality that we do not have the capacity for expert technical mentoring from non-technical founders, we require volunteers to use LeetCode as a standardized, non-biased tool for skill improvement assessment.

* **Monthly Goal:** Volunteers must successfully complete and submit evidence of **at least one (1) LeetCode challenge per calendar month.**  
* **Purpose:** This serves as a consistent marker of tangible progress in fundamental data structures, algorithms, and problem-solving skills, and helps ensure skill improvement is occurring even without direct expert oversight.  
* **Accountability:** Completion of the monthly challenge is a core requirement for demonstrating ongoing commitment and skill development within the upskilling project.

## **4\. Policy Enforcement and Support**

* **Mentorship:** Project mentors are available to provide support. We encourage volunteers to approach mentors with specific questions about AI-generated code to deepen their understanding of its mechanics.  
* **Violation:** Repeated failure to adhere to the Verification (V) and Intention-First Learning (I) principles, especially a lack of demonstrable understanding of submitted code, will lead to remedial mentoring or a review of your participation status.  
* **Continuous Feedback:** This policy is a living document and will be reviewed regularly to ensure it supports the development of strong, independent programming skills among all volunteers.
