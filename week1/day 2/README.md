# Day 2: Platform Basics

## 1. What is the Salesforce Platform?
**Salesforce Platform** is a cloud-based platform that lets businesses build applications, manage customer data, and automate processes—all in one place.

---

## 2. Core Concepts Explained

*   **App:** Imagine an App as a dedicated workspace or a folder for a specific job. It’s a collection of items (like tabs and dashboards) grouped together to help users complete a specific process (e.g., a "Recruiting" or "Sales" app).
*   **Object:** If Salesforce is a giant Excel workbook, an **Object** is a single spreadsheet tab within it. It’s a database table that stores specific information (e.g., a "Student" object).
*   **Tab:** A **Tab** is the clickable shortcut at the top of your screen. It’s the user interface element that lets you view the data stored inside an Object.

---

## 3. Configuration vs. Coding


| Feature | Type | Analogy |
| :--- | :--- | :--- |
| **Configuration** | **Clicks** | Like building with **Lego blocks**. You use drag-and-drop tools and menus to build the system without writing code. |
| **Coding** | **Code** | Like **3D printing** your own custom Lego blocks. Developers use **Apex** or **JavaScript** for complex requirements. |

---

## 4. Real System Thinking: College Admission System

Based on my standard object mapping, here is how I would design the **Admissions Hub** app:

### 📱 App Details
*   **App Name:** Admissions Hub
*   **Purpose:** To manage the end-to-end student recruitment and enrollment process.

### 📦 Objects Inside the App
*   **High Schools (Account):** The institution the student is coming from.
*   **Students (Contact):** The individual person applying for a degree.
*   **Applications (Opportunity):** Tracking the student from "Applied" to "Admitted" or "Enrolled."
*   **Prospective Students (Lead):** People who inquired but haven't applied yet.
*   **Campus Tours (Custom Object):** A custom table to track campus visit dates.

### 🔄 How Users Interact
1.  **Recruiters** log in and check the **Prospective Students** tab for new inquiries.
2.  When a student applies, the recruiter **converts** them into a **Student**.
3.  **Reviewers** use the **Applications** tab to move the stage from "Under Review" to "Admitted."

## progress
<img width="1907" height="868" alt="Screenshot 2026-05-09 194933" src="https://github.com/user-attachments/assets/9f69751a-e6da-4ccc-bb79-5433ee315199" />
<img width="1877" height="980" alt="Screenshot 2026-05-09 192004" src="https://github.com/user-attachments/assets/d5e153b8-292b-44b0-bad6-fdcba1c0c41a" />
<img width="1896" height="944" alt="Screenshot 2026-05-10 102442" src="https://github.com/user-attachments/assets/4d00ea9d-11ee-446a-a9b0-2c1c41403cfd" />
<img width="1912" height="972" alt="Screenshot 2026-05-09 232358" src="https://github.com/user-attachments/assets/30c26d96-f036-462e-920d-a2a3b5d03f4b" />
<img width="1909" height="974" alt="Screenshot 2026-05-09 231801" src="https://github.com/user-attachments/assets/464fce0b-8ddc-49c3-985e-5dd8571fb754" />
<img width="1903" height="971" alt="Screenshot 2026-05-09 225626" src="https://github.com/user-attachments/assets/49196e63-5350-437d-8ef0-8eaaf9dd5d87" />
<img width="1596" height="972" alt="Screenshot 2026-05-09 225616" src="https://github.com/user-attachments/assets/47e3a9bf-daca-46e1-a399-4561ebf0742d" />
<img width="1912" height="972" alt="Screenshot 2026-05-09 224557" src="https://github.com/user-attachments/assets/b4c9f66d-ea50-464d-b49a-a98738006f2b" />


