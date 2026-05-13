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


	<img width="1911" height="1006" alt="image" src="https://github.com/user-attachments/assets/8b90c805-d39d-4d6d-b373-63c1a8f382dc" />

2.	a.	Name: e.g., Nigerian BVN
	 
    b.	Description
  	 	<img width="1362" height="621" alt="Screenshot 2026-05-13 180240" src="https://github.com/user-attachments/assets/22480732-7560-4794-b17a-af2360e34267" />
    
3.	Create a pattern:

	
a.	Primary element = Regular Expression → choose from existing regular expressions
<img width="1365" height="618" alt="Screenshot 2026-05-13 184110" src="https://github.com/user-attachments/assets/fd733bf7-3edf-4eb2-a633-86e236868a4a" />
 <img width="837" height="267" alt="Screenshot 2026-05-13 192238" src="https://github.com/user-attachments/assets/39142b02-99af-46a7-9235-3d02456c84d8" />

<img width="1359" height="609" alt="Screenshot 2026-05-13 184416" src="https://github.com/user-attachments/assets/fcfc35a1-9a08-42b5-98d0-cc9805a23d53" />

<img width="1360" height="608" alt="Screenshot 2026-05-13 190651" src="https://github.com/user-attachments/assets/416a26bb-ad77-468e-974c-2779e785af5d" />


b.	Optional = Validator or Keyword list
<img width="1363" height="611" alt="Screenshot 2026-05-13 185825" src="https://github.com/user-attachments/assets/1e549f44-c21a-4b63-982c-a064f5a1e68c" />
<img width="1357" height="610" alt="Screenshot 2026-05-13 190413" src="https://github.com/user-attachments/assets/eea7925a-0880-49bd-b1fa-5cddbfdbf563" />
<img width="1362" height="604" alt="Screenshot 2026-05-13 191502" src="https://github.com/user-attachments/assets/5f4fa5b7-de72-4223-b400-217061644854" />

4.	Set confidence level (Medium or High).
   <img width="1360" height="601" alt="Screenshot 2026-05-13 192747" src="https://github.com/user-attachments/assets/663a1e96-6961-4d2b-b95b-4e6fc42dc3c0" />

   Review settings and finish
   
   <img width="1362" height="601" alt="Screenshot 2026-05-13 192808" src="https://github.com/user-attachments/assets/a5192096-24a0-46f4-a32e-d6b44ed209d1" />
   
<img width="1357" height="603" alt="Screenshot 2026-05-13 192836" src="https://github.com/user-attachments/assets/324c5c26-e794-4ce0-8635-47d7bf556ca0" />

## # Testing the SIT
•  Use the Test feature in Purview to upload a sample file containing the bank account numbers or BVNs.
•  Adjust regex or supporting evidence until detection is reliable.

<img width="1363" height="618" alt="1" src="https://github.com/user-attachments/assets/962f1446-a5f5-47c1-9c37-0fc5d303cf35" />

<img width="1356" height="604" alt="2" src="https://github.com/user-attachments/assets/346fb38b-95bb-4210-8b89-d9a164c6eff2" />

<img width="1355" height="601" alt="3" src="https://github.com/user-attachments/assets/9e24e5f4-889f-4897-b945-892e5f9a3752" />

<img width="1355" height="601" alt="4" src="https://github.com/user-attachments/assets/e699d86c-217a-467b-be39-54168171d400" />



# 2. Once the SITs exist, create a Sensitivity Label that automatically applies when the SIT is detected.
## Steps
1.	Go to Purview → Information Protection → Labels → Create a label.
	<img width="1364" height="607" alt="Screenshot 2026-05-13 200816" src="https://github.com/user-attachments/assets/9887f7de-e224-4f84-b58f-f22d0e624ec2" />

2.	Configure:
    Name: e.g., Finance – Restricted
  	<img width="1360" height="602" alt="Screenshot 2026-05-13 201357" src="https://github.com/user-attachments/assets/2925bbc6-7e57-4a48-a3d6-7c483fb30663" />

3.	Scope: Files & Emails
   <img width="973" height="403" alt="image" src="https://github.com/user-attachments/assets/ffc26785-0b7c-47f2-b771-ebcffb9c24fa" />
4. Access control
   <img width="1360" height="605" alt="Screenshot 2026-05-13 202032" src="https://github.com/user-attachments/assets/542498e8-a3ca-4e18-b552-c162e3fd31c0" />

5. Auto-labeling for files and emails
   <img width="1348" height="606" alt="Screenshot 2026-05-13 202455" src="https://github.com/user-attachments/assets/08f5f4a4-5bfe-432a-8b7c-c33109e05a4f" />

   6. New sensitivity label created
      <img width="1360" height="608" alt="Screenshot 2026-05-13 202656" src="https://github.com/user-attachments/assets/ffbbc45e-43e1-419b-9d9a-b27176801cc7" />

      7. Setting up Auto-labeling policies
         <img width="1354" height="609" alt="Screenshot 2026-05-13 203006" src="https://github.com/user-attachments/assets/e7d39f59-f818-4901-a61f-b0dfbbcc733e" />

<img width="1363" height="610" alt="Screenshot 2026-05-13 203406" src="https://github.com/user-attachments/assets/c28112b6-177a-4b23-9ea0-e678a42dbc07" />

<img width="1357" height="604" alt="Screenshot 2026-05-13 203900" src="https://github.com/user-attachments/assets/32e4c64a-edfd-4bc4-a4b5-d6b7e73a8271" />

 
