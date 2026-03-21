# **Best Practices for UI Screenshot Documentation**

| Field | Value |
| :---- | :---- |
| **Document ID** | GUIDE-20251023-021 |
| **Filepath** | docs/project\_mgmt/screenshot\_guidance.md |
| **Document Title** | Screenshot Documentation Guide |
| **Date** | 2025-10-23 |
| **Version** | 1.0 |
| **Status** | Finalized |

## **1\. Where to Store Screenshots**

Screenshots should **never** be stored directly in the root of the repository or alongside source code. They belong in a dedicated, centralized folder for all non-code assets.

| Rule | Location | Rationale |
| :---- | :---- | :---- |
| **Standard Folder** | docs/assets/screenshots/ | Keeps the root clean and separates large binary files from documentation and source code. |
| **Naming Convention** | Use lowercase, hyphens, and include the version or feature name (e.g., ftm-v1-transaction-view.png). | Ensures consistency and makes files easy to reference and search. |
| **File Type** | **PNG** for UI elements (sharp lines, text) and **JPG** for realistic photos or complex images (smaller file size). | PNG is lossless and ideal for capturing application interfaces cleanly. |

## **2\. When to Include Visuals (Use Cases)**

Screenshots should be used strategically to support documentation, not replace it.

### **A. README and High-Level Summaries**

* **Purpose:** To give new users or developers a quick visual overview of the application's core functionality.  
* **What to include:** The main dashboard, the most impressive/complex feature, or the mobile view.

### **B. Feature Specification Documents (SSDDs)**

* **Purpose:** To lock in the design and interaction for a feature before coding begins or to document the final implemented state.  
* **What to include:** Before-and-after views, complex interaction flows (e.g., a multi-step form), or views showing critical data points (like the FTM transaction screen).

### **C. Pull Requests (PRs)**

* **Purpose:** The most frequent use case. Every UI-related pull request should include a screenshot or a GIF/video demonstrating the change.  
* **What to include:** A clear visual comparison showing the difference your code introduced.

## **3\. Quality and Style Guidelines (Consistency is Key)**

Maintaining a consistent style makes your documentation look professional and trustworthy.

### **A. Cropping and Padding**

* **Focus on the Feature:** Crop tightly around the feature you are documenting. Do not include unnecessary browser tabs, operating system elements, or desktop backgrounds.  
* **Maintain Padding:** If possible, ensure 20-30 pixels of padding around the main element to prevent the image from looking "cut off."

### **B. Annotations and Highlighting**

* **Avoid Over-Marking:** Use simple boxes or arrows to draw attention to specific elements. Avoid overly busy or colorful annotations.  
* **Blur Sensitive Data:** **Mandatory:** Always blur or obscure any sensitive information, placeholder names, real emails, or financial figures before committing a screenshot. Use mock data where possible.

### **C. Mobile vs. Desktop**

* When documenting a feature, include **both** the desktop view and the corresponding mobile view to ensure the responsiveness is clearly understood and recorded.
