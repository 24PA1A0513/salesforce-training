# 🏛️ Salesforce Data Modeling: College Management System

This repository tracks the architecture of our **"Campus Connect"** application, detailing how core platform principles organize and protect academic data.

---

## 📁 1. Core Concepts: The Filing System Analogy

*   **App (The Cabinet):** Tailored workspace for specific workflows (e.g., Admissions Hub).
*   **Object (The Folders):** Database tables storing distinct data pools (e.g., `Student__c`).
*   **Record (The Documents):** Individual entries inside a table (e.g., Student "Thafil").
*   **Field (The Blank Lines):** Columns storing specific data attributes (e.g., `Email`, `GPA`).

---

## ⚙️ 2. Standard vs. Custom Objects

*   **Standard Objects:** Built-in tables provided out-of-the-box by Salesforce (e.g., `Account`, `Contact`).
*   **Custom Objects:** Unique tables created for specific business needs (e.g., `Professor__c`). These are marked by the `__c` API suffix.

---

## 🔗 3. Data Model & Relationships

Our architecture handles academic tracking using specialized link relationships to connect objects safely:

### 🔹 One-to-Many Connections (Lookups)
*   **Department to Professor:** Tracks which department manages which faculty members.
*   **Professor to Course:** Assigns specific instructors to their respective classes.

### 🔹 Many-to-Many Connections (Junction Object)
*   **Student to Course:** Connected via a dedicated junction object named **`Enrollment__c`**.
*   This junction uses independent **Master-Detail** relationships linking both objects.

---

## 🧮 4. Formula Fields

Formula fields process entries dynamically and remain strictly read-only:

*   **Full Name (Text):** Combines first and last names with clean spacing.
    ```sql
    First_Name__c & " " & Last_Name__c
    ```
