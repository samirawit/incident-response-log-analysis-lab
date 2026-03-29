# Windows Failed Login Analysis (Event ID 4625)

This project focuses on analyzing failed login attempts using Windows Event Viewer. The goal was to better understand how authentication failures appear in system logs and identify any suspicious patterns.

## Objective
Review Windows Security logs to identify failed login attempts and determine whether the activity could indicate a potential security risk.

## Tools Used
- Windows Event Viewer

## What I Did
- Generated multiple failed login attempts by entering incorrect passwords  
- Navigated to the Security logs in Event Viewer  
- Filtered logs using Event ID 4625  
- Reviewed details such as account name, logon type, failure reason, and timestamps  

## Key Findings
- Multiple failed login attempts occurred within seconds  
- All attempts targeted the same user account  
- Logon Type 2 (interactive login) was used  
- All failures were due to incorrect password entry  

## Analysis
The repeated login attempts within a short time frame suggest more than a one-time mistake. While this could be user error, the pattern could also indicate a potential brute-force or unauthorized access attempt.

## Framework Mapping
This activity aligns with the following NIST 800-53 controls:
- AC-7 (Account Lockout)  
- AU-2 (Audit Events)  
- AU-6 (Audit Review and Analysis)  
- SI-4 (System Monitoring)  
- IR-4 (Incident Handling)
