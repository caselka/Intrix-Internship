# PortSwigger Web Security Academy Labs ✅

## Overview
The **PortSwigger Web Security Academy** provides hands-on **web security training**. This week, I completed **SQL Injection** and **XSS** labs.

## Lab 1: SQL Injection (Basic)
**Objective:**  
- Exploit a **login form** using SQL injection (`' OR 1=1 --`).
- Gain **unauthorized access** to the application.

**Steps Taken:**
1. **Tested input field** with `GET /filter?category='+OR+1=1-- HTTP/1.1`.
2. The SQL query **bypassed authentication**.
3. Made changes without logging in **without credentials**.

**Screenshot:**  
Is in Screenshots for Pen Testing (sql-injection-lab.png)

## Lab 2: Cross-Site Scripting (XSS)
**Objective:**  
- Inject JavaScript into a vulnerable **search field**.
- Trigger an **alert box**.

**Steps Taken:**
1. Entered the payload:  
   ```html
   <script>alert("Hacked")</script>
