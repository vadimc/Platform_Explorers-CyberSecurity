# Protect sensitive financial information including personal data, financial records and intellectual property from unauthorized access and data breaches

## Platform Explorers – Cybersecurity
## Cyber Security Analyst: Vadim Caraman
## Microsoft Security Platform: Microsoft Purview

# Overview  
This use case outlines the process for a company to implement Microsoft Purview Sensitivity Labels specifically for the finance department. The goal is to automatically label financial information and prevent the finance team from sending emails and documents containing this type of information outside the department or with AI solutions like M365 Copilot.

# Requirements: 
## Sensitive Information Type (SIT): 
Create a custom SIT to classify a type of financial data. For example Croatian Bank account number, Nigerian BVN, and test the SIT using a sample test file.
##  Sensitivity Labels: 
Create a Sensitivity label to apply to emails and files if the SIT created earlier is found.

## DLP Policies: 
Prevent the finance team from using M365 Copilot to process information related to the SIT earlier created.

## You can meet all three requirements—custom SIT, auto labeling, and blocking Copilot—by combining Microsoft Purview Sensitive Information Types, Sensitivity Labels, and DLP policies. Below is a complete, structured implementation plan.

# 1. Create Custom Sensitive Information Types (SITs)
Microsoft Purview allows you to define custom SITs using regex, keyword lists, or validation logic. This is required because Croatian bank account numbers and Nigerian BVNs are not built in types.

# Steps
1.	Go to Microsoft Purview Portal → Information Protection → Classifiers → Sensitive info types → Create sensitive info type. 
2.	Define:
3.	<img width="1911" height="1006" alt="image" src="https://github.com/user-attachments/assets/8b90c805-d39d-4d6d-b373-63c1a8f382dc" />

4.	a.	Name: e.g., Nigerian BVN 
    b.	Description
  	<img width="1362" height="621" alt="Screenshot 2026-05-13 180240" src="https://github.com/user-attachments/assets/22480732-7560-4794-b17a-af2360e34267" />
3.	Create a pattern:
a.	Primary element = Regular Expression → choose from existing regular expressions
<img width="1365" height="618" alt="Screenshot 2026-05-13 184110" src="https://github.com/user-attachments/assets/fd733bf7-3edf-4eb2-a633-86e236868a4a" />
b.	Optional = Validator or Keyword list




