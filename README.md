# SQL-Injection-PortsSwigger
Documenting my learning journey for SQL Injection
## PortSwigger Web Academy - SQL Injection

### Lab 1: SQL Injection in WHERE Clause
**Date:** 24/02/2026

### What I Did
- Injected '+OR+1=1-- into the query parameter
- 1=1 is always true so the database returned all records including hidden ones

### Lab 2: SQL Injection Login Bypass
**Date:** 24/02/2026

### What I Did
- Injected '-- after the username field
- -- comments out the rest of the query so the password check never executes
- Bypassed authentication without knowing the password

### Key Takeaways
- SQL injection works by manipulating unsanitized input fields to alter database queries
- Always true conditions return unintended data
- Comment operators can eliminate security checks entirely
