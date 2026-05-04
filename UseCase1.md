
# Mitigating Fraudulent Emails at Contoso

## Cyber Security Analyst: Vadim Caraman  
## Platform Explorers – Cybersecurity  
## Microsoft Security Platform: Microsoft Defender for Office 365  
---

#  Company Overview:
Contoso is a mid-sized organization with 300 users located in the United States and Western Europe. The company has been experiencing a significant challenge with fraudulent emails being delivered to end users' mailboxes, posing a risk of phishing attacks and potential data breaches.

## Solution :
- Create  Inbound Anti‑Spam Policy for Contoso end user’s mailboxes in  **Microsoft Defender for Office 365**
* Defender for office 365 - email&collaboration - policies and rules - threat policies – anti fishing policy -  +create - policy name - users, groups and domains - phishing threshold & protection - actions - review - done
## Step1
<img width="939" height="436" alt="image" src="https://github.com/user-attachments/assets/6ad6eb64-9067-4414-925a-52b6763461a8" />

 
(FYI, do not use any special characters for policy name/description as you will end up with an error)

## Step2 
<img width="939" height="425" alt="image" src="https://github.com/user-attachments/assets/af5f796d-51d8-483f-93b2-4c1376f0c73b" />
We exclude the CEO & CFO as they need to be on a separate policy
 
 <img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/4151eee9-4781-4fa5-a440-d0cab450d3f3" />

# Step3 
<img width="939" height="418" alt="image" src="https://github.com/user-attachments/assets/6dfee872-ee0e-45f1-9416-218fcce774d7" />
<img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/39566cc7-a47e-4eb6-a6f3-1a6222df133d" />

# Step4
   <img width="939" height="434" alt="image" src="https://github.com/user-attachments/assets/00df6506-2888-456d-ac5c-ae128df75ec3" />
<img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/42d9ed25-75aa-48fb-be3f-049f80160574" />

<img width="939" height="429" alt="image" src="https://github.com/user-attachments/assets/83c9629f-ddbd-4cc5-899d-648cb9f8fe15" />

# Step5
 <img width="939" height="427" alt="image" src="https://github.com/user-attachments/assets/6527bc46-c0c6-4a05-9a30-96e5b9bf136e" />


# Step6
 <img width="938" height="429" alt="image" src="https://github.com/user-attachments/assets/7a6119fc-e21d-4c3f-83cd-c8c5c83366d3" />

 <img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/935bcaed-20ac-41d4-ae8b-36edbd156a5f" />


# Problem Statement:
Contoso's email system is currently vulnerable to fraudulent emails, which are being delivered to end users' mailboxes. This issue has raised concerns about the security of sensitive information and the potential for phishing attacks. The company needs to implement a robust solution to mitigate this risk and protect its users, especially VIP users such as the CEO, CFO, and CISO.


# Create Anti-Spam policy to protect CEO and CFO

* Defender for office 365 - email&collaboration – anti spam policy -  policies and rules - threat policies – anti-spam policy -  +create inbound policy - policy name - users, groups and domains - threshold & protection - actions - review - done

# Step1 
<img width="938" height="427" alt="image" src="https://github.com/user-attachments/assets/d67bcbaa-318a-4f3b-b82c-5fc760a9a454" />


# Step2
 <img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/09f8cadb-d648-4c63-ae5d-55488065b0b2" />


#Step3
 <img width="939" height="432" alt="image" src="https://github.com/user-attachments/assets/23342044-7e79-470f-a1d6-42c6188cff3b" />

# Step4
  <img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/3d917e3a-35c2-46aa-877b-7315b94f16f1" />
 
<img width="939" height="432" alt="image" src="https://github.com/user-attachments/assets/3eb38aeb-dd4e-479d-b94b-314e484f6d5d" />
<img width="939" height="427" alt="image" src="https://github.com/user-attachments/assets/ee219e87-01e8-4c94-a638-86ffb1c5a889" />

# Step5
 <img width="939" height="427" alt="image" src="https://github.com/user-attachments/assets/20c180f3-c018-42b2-bbf4-f7fb50fa5634" />


# Step6
  <img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/f2804e3c-0b0b-4e9a-8e13-2a940787ca33" />
<img width="939" height="423" alt="image" src="https://github.com/user-attachments/assets/46bcccfb-dbe9-42f8-87c0-077ac54d12b8" />

#Step7
  
<img width="939" height="425" alt="image" src="https://github.com/user-attachments/assets/eaf83107-38fb-4466-b81d-9536bbf7bc18" />
<img width="938" height="421" alt="image" src="https://github.com/user-attachments/assets/2b69ea14-4679-4517-a72f-32dcbbd87607" />


# GTUBE Spam Test
i.	Sender: my personal gmail
ii.	Recipient: PradeepG@platexp.onmicrosoft.com 
iii.	                   AdeleV@platexp.onmicrosoft.com
iv.	Subject: GTUBE spam filter test
v.	Body  (must be on a single line): XJS*C4JDBQADN1.NSBN3*2IDNEN*GTUBE-STANDARD-ANTI-UBE-TEST-EMAIL*C.34X

 
<img width="939" height="388" alt="image" src="https://github.com/user-attachments/assets/81d74b78-50dc-4988-a91a-19ec2ffdbc11" />
<img width="939" height="407" alt="image" src="https://github.com/user-attachments/assets/1f9dc0d1-158f-4c35-97cd-4416057908ba" />

 

# Objective:
To seek advice from a security analyst on the resolution of the fraudulent email issue, including the type of Microsoft 365 plan that can be purchased, features that can help mitigate the concern, and configuration steps that can be taken to protect the organization.
The analyst needs to configure their recommended policies to solve the business problem.
Additionally, the analyst should take screenshots of the configuration steps and upload them to their GitHub repository, explaining their thought process and any potential implications of the new policies.
The analyst should also determine if these steps should be applied to a group of test users first before being rolled out to the entire organization, ensuring the protection of VIP users.
Also, the analyst should advise on how to get mail flow reports which can be shared with stakeholders.

# Solution :

	A strong, clear path forward is to harden Contoso’s email environment with layered, identity‑aware protections that stop fraudulent messages before they ever reach users—especially VIPs who are prime targets. The core issue is classic: attackers are bypassing existing controls, exploiting gaps in authentication, and relying on human trust. The solution is a combination of email authentication, advanced threat detection, and VIP‑focused protections.


1. Implement and enforce DMARC, SPF, and DKIM
These three protocols work together to verify that incoming mail is legitimate.
SPF — Confirms which servers are allowed to send mail for your domain.
DKIM — Cryptographically signs messages so recipients can verify authenticity.
DMARC — Tells receiving servers what to do with messages that fail SPF/DKIM.
Critical step: Move DMARC from none → quarantine → reject once alignment is confirmed.
This alone eliminates a huge portion of spoofed email.

## VIP‑Focused Protection: CEO, CFO, CISO
Executives are disproportionately targeted because they have:

High authority

Access to sensitive data

Influence over financial decisions

## Create a VIP protection policy
This should include:

Dedicated impersonation protection for their names, roles, and domains

Higher‑sensitivity anti‑phishing thresholds

Automatic quarantine for suspicious messages

Enhanced logging and alerting for any anomalies

Conditional Access requiring phishing‑resistant MFA (FIDO2, Windows Hello for Business)

## Human Layer: Reduce Risk Through Training
Even the best technical controls can’t eliminate human error.

Conduct targeted phishing simulations
Focus on:

Wire‑transfer fraud

Executive impersonation

Urgent “CEO requests”

Fake document‑sharing notifications

## Provide VIP‑specific awareness sessions
Executives often bypass training due to time constraints, but they are the highest‑risk group. Tailored, short sessions are essential.



## Enable continuous access evaluation
This cuts off compromised sessions in real time.

   Optional but High‑Value Enhancements
These add resilience and visibility:

External email tagging (“This message came from outside Contoso”)

Brand Indicators for Message Identification (BIMI)

Threat intelligence integration

Automated incident response playbooks

Domain monitoring for lookalike registrations




