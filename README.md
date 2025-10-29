# API 6th Semester DB

# PRO4TECH - LuminIA

<p align="center">
      <img src="docs/Logo LuminIA.jpeg" alt="logo_projeto" width="200">
      <h2 align="center"> LuminIA </h2>
</p>

<p align="center">
 |<a href ="#challenge"> Challenge </a>  |
  <a href ="#solution"> Solution </a>  | 
  <a href ="#non_functional_requirements"> Non-Functional Requirements </a>  |
  <a href ="#functional_requirements"> Functional Requirements </a>  |
  <a href ="#backlog"> Product Backlog </a>  |
  <a href ="#dor"> DoR </a>  |
  <a href ="#dod"> DoD </a>  |
  <a href ="#sprint"> Sprint Schedule </a>  |
  <a href ="#technologies"> Technologies </a> | 
  <a href ="#burndown"> Burndown</a> | 
  <a href ="#team"> Team</a> |
  <a href ="#more_information"> More Information </a> |
</p>

> Project Status: Under development... 🚧 
>
> Test Report: Under development... 🚧 📊
>
> Documentation Folder: Under development... 🚧 [Link](https://github.com/new-ge/LuminIA/wiki) 📄
>
> Project Video: [Youtube](https://www.youtube.com/watch?v=0wkynwCSBhQ&list=PLHVGmwwpPVx5gGkzYJdrJ0NI2eazVkwds&pp=gAQB) 📽️  

---

## 🏅 Challenge <a id="challenge"></a>

## Challenge Description  

The current situation shows that the support database no longer meets operational needs: it does not fully guarantee compliance with the law, does not provide enough clarity for audits, and does not facilitate historical or predictive analysis. This means reports end up being rigid and repetitive, without giving a complete view for decision-makers. The modernization proposal seeks to address these limitations, bringing more security in data handling, transparency in monitoring actions, and dashboards that help every level of the team — from analysts to managers and strategic stakeholders — to visualize exactly the information they need to work more efficiently.  

---

## 🏅 Solution <a id="solution"></a>

LuminIA is an integrated AI-powered dashboard carefully developed to facilitate and optimize management decision-making, while continuously supporting analysts in handling tickets. With strategic insights and AI reinforcement, LuminIA transforms complex information into concrete actions, making the entire support process more efficient, agile, intelligent, and aligned with business needs. All of this is provided through a modern, intuitive, and easy-to-use tool, designed so managers and analysts can quickly access data. 

---

## Non-Functional Requirements <a id="non_functional_requirements"></a>

| **ID** | **Title** |
|:------:|:---------:|
| RNF01  | Compliance with LGPD (anonymization/pseudonymization of sensitive data) |
| RNF02  | Prepared base for historical analysis |
| RNF03  | Responsive interface (web and mobile) |
| RNF04  | AI ticket analysis |
| RNF05  | Access level structure |
| RNF06  | User Manual |
| RNF07  | Database Modeling |

---

## Functional Requirements <a id="functional_requirements"></a>

| **ID** | **Persona**   | **Title**                   | **Description** |
| :------: | :-------------: | :---------------------------: | :---------------: |
| R1     | Analyst       | Average lead time           | The system should display a card showing the **average lead time**, allowing the Analyst (N1, N2, or N3) to analyze their team’s performance, specifically the average time gained per resolved or closed ticket. |
| R2     | Analyst       | Recurring tickets volume    | The system should display a card showing the **number of recurring tickets**, allowing the Analyst (N1, N2, or N3) to analyze team performance by identifying cases marked as resolved or closed that returned to a previous status. |
| R3     | Analyst       | Negative tickets volume     | The system should display a chart showing the **number of poorly rated tickets**, providing awareness of demand. |
| R4     | Analyst       | Tickets volume by period    | The system should display a chart showing the **number of tickets over selectable periods**, allowing the Analyst to analyze team performance retroactively. |
| R5     | Analyst       | SLA filter                  | The system should allow the Analyst to apply an **SLA filter** on tickets, showing feedback in cards and charts by customer type: Standard, VIP, or Extended. |
| R6     | Analyst       | Status filter               | The system should allow the Analyst to apply a **status filter**, showing feedback in cards and charts by ticket status: Open, In Progress, Waiting for Customer, Resolved, and Closed. |
| R7     | Analyst       | Priority filter             | The system should allow the Analyst to apply a **priority filter**, showing feedback in cards and charts by priority: Low, Medium, High, and Critical. |
| R8     | Analyst       | Subcategory filter          | The system should allow the Analyst to apply a **subcategory filter**, showing feedback in cards and charts by subcategory: System Error, Slowness, Unavailable Functionality, Login Issues, Permissions, User Registration, Reports, Export, and Inconsistent Data. |
| R9     | Analyst       | Period filter               | The system should allow the Analyst to apply a **period filter**, providing feedback in cards and charts between two dates. |
| R10    | Product Owner | Total open tickets          | The system should display a card showing the **total number of open tickets** across all supervised teams, to analyze demand status. |
| R11    | Product Owner | Tickets volume by period    | The system should display a chart showing the **number of tickets over selectable periods** across all supervised teams, to analyze demand over time. |
| R12    | Product Owner | Average resolution time     | The system should display a chart or card with the **average time taken to resolve tickets** across all supervised teams, to analyze average resolution performance. |
| R13    | Product Owner | SLA exceeded tickets        | The system should display a card identifying **tickets exceeding SLA** across all supervised teams, to analyze delays. |
| R14    | Product Owner | Recurring tickets volume    | The system should display a chart or card with the **number of recurring tickets** across all supervised teams. |
| R15    | Product Owner | Sentiment analysis          | The system should display a chart showing the **number of poorly rated tickets** across all supervised teams. |
| R16    | Product Owner | SLA filter                  | The system should allow the PO to apply an **SLA filter**, showing feedback in cards and charts by customer type: Standard, VIP, or Extended. |
| R17    | Product Owner | Team filter                 | The system should allow the PO to apply a **team filter**, showing feedback in cards and charts by selected team. |
| R18    | Product Owner | Status filter               | The system should allow the PO to apply a **status filter**, showing feedback by ticket status: Open, In Progress, Waiting for Customer, Resolved, and Closed. |
| R19    | Product Owner | Period filter               | The system should allow the PO to apply a **period filter**, showing feedback in cards and charts between two dates. |
| R20    | Product Owner | Priority filter             | The system should allow the PO to apply a **priority filter**, showing feedback in cards and charts by priority: Low, Medium, High, and Critical. |
| R21    | Product Owner | Subcategory filter          | The system should allow the PO to apply a **subcategory filter**, showing feedback in cards and charts by subcategory. |
| R22    | Product Owner | Tag filter                  | The system should allow the PO to apply a **tag filter**, showing feedback in cards and charts by tag: Urgent, Review, Bug, Request, Improvement, Finance, HR, IT, Duplicate, and Follow-up. |
| R23    | Manager       | Global data access          | The system should display all charts, cards, and filters available to the PO level, but managers will have access to all teams. |
| R24    | Admin         | User and permission management | Allow the administrator to: <br>• Create, edit, and delete users.<br>• Define profiles and permissions by hierarchy level.<br>• Ensure users only see authorized data.<br>• Delete user data when requested (LGPD compliance). <br>**Expected behavior:** logs of creation, editing, and deletion of users. |
| R25    | Admin         | Detailed logs               | Store **complete logs of all operations**, including login/logout, data changes, deletions, report access, and filters applied. <br>**Objective:** ensure traceability and audit. |
| R26    | Analyst N1    | FAQ                         | Provide an **automated FAQ** for Level 1 Analysts. |
| R27 | Analyst | Opened tickets volume | The system should display a card showing the number of open tickets, allowing the Analyst (N1, N2, or N3) to work on unresolved cases and track team performance. |
| R28 | Analyst | Tickets exceeding SLA volume | The system should display a card showing the number of tickets exceeding SLA, allowing the Analyst (N1, N2, or N3) to identify priority issues and act quickly to reduce delays in service. |

---

## 📋 Product Backlog <a id="backlog"></a>

| Rank | Epic | Priority | User Story | Sprint | Story Points | Status | Requirements |
|:------:|:------------------------------------:|:----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------:|:--------------:|:--------------:|:---------------------:|
| 1    | AI Support Indicators Dashboard   | High     | As a support analyst N1, I want to provide a FAQ with answers to the most common customer questions, so that I can reduce repetitive tickets and speed up service. | 2        | 8            | Done  | R26, RNF04         |
| 2    | AI Support Indicators Dashboard   | High     | As a support manager, I want to view the volume of open tickets so I can know how many tickets still need attention.                                               | 1        | 4            | Done    | R23, RNF02         |
| 3    | AI Support Indicators Dashboard   | High     | As a support manager, I want to view ticket volume over time with an AI-generated trend line so I can identify peaks and anticipate which types of tickets are more likely to occur. | 1        | 11           | Done    | R23, RNF04         |
| 4    | AI Support Indicators Dashboard   | High     | As a support manager, I want to view average ticket resolution time so I can know whether service meets expected standards.                                        | 1        | 4            | Done    | R23                 |
| 5    | AI Support Indicators Dashboard   | High     | As a support manager, I want to view the volume of tickets that exceeded SLA so I can identify delays, take corrective action, and improve support efficiency.     | 1        | 4            | Done    | R23                 |
| 6    | AI Support Indicators Dashboard   | High     | As a support manager, I want to view recurring ticket volume so I can identify recurring problems, reduce rework, and improve customer satisfaction.              | 1        | 4            | Done    | R23, RNF02         |
| 7    | AI Support Indicators Dashboard   | High     | As a support manager, I want to view sentiment volume using AI analysis so I can identify patterns and quickly detect critical tickets.                           | 1        | 9            | Done    | R23, RNF04         |
| 8    | AI Support Indicators Dashboard   | High     | As a support manager, I want to filter by SLA plans, team, status, period, priority, subcategory, and tag so I can analyze segmented data and make better decisions. | 1        | 28           | Done    | R23                 |
| 9    | AI Support Indicators Dashboard   | High     | As a support analyst, I want to view average lead time so I can understand if I am resolving tickets early enough.                                                 | 2        | 3            | Done  | R1                  |
| 10   | AI Support Indicators Dashboard   | High     | As a support analyst, I want to view recurring ticket volume so I can identify how many issues return and improve service quality.                                 | 2        | 3            | Done  | R2                  |
| 11   | AI Support Indicators Dashboard   | High     | As a support analyst, I want to view sentiment-negative ticket volume using AI analysis so I can identify patterns and act on critical tickets.                  | 2        | 3            | Done  | R3, RNF04          |
| 12   | AI Support Indicators Dashboard   | High     | As a support analyst, I want to view ticket volume by period so I can analyze demand and detect peaks.                                                             | 2        | 3            | Done| R4                  |
| 13   | AI Support Indicators Dashboard   | High     | As a support analyst, I want to filter by SLA plans, status, priority, subcategory, and period so I can analyze segmented data and improve service.               | 2        | 4            | Done  | R5, R6, R7, R8, R9 |
| 14   | Access Management                  | Medium   | As an administrator, I want to create different access levels so I can control who can see data.                                                                  | 3        | -            | In Progress  | R23, RNF05         |
| 15   | Administration                     | Medium   | As an administrator, I want to delete users so I can revoke access to the application.                                                                             | 3        | -            | In Progress  | R24, RNF05         |
| 16   | Administration                     | Medium   | As an administrator, I want to create users so I can grant access to the application.                                                                             | 3        | -            | In Progress  | R24, RNF05         |
| 17   | Administration                     | Medium   | As an administrator, I want to edit users so I can change user information.                                                                                       | 3        | -            | In Progress  | R24, RNF05         |
| 18   | Login                              | Low      | As a system user, I want to log in with secure credentials so I can access only authorized features.                                                               | 3        | -            | In Progress  | RNF05               |
| 19   | Data Modernization                  | High     | As a system user, I want data modernization so I can access data more easily.                                                                                      | 1        | 3            | Done    | RNF07               |
| 20   | Data Modernization                  | High     | As a system user, I want my personal data handled in compliance with LGPD so I have security, transparency, and control over my data.                              | 2        | 3            | In Progress  | RNF01               |
| 21   | User Manual                        | High     | As a system user, I want a user manual so I can learn how to use the application.                                                                                  | 3        | -            | In Progress  | RNF06               |
22 | AI Support Indicators Dashboard | High | As a support analyst, I want to view open tickets so that I can work on unresolved cases. | 2 | 3 | Done | R27
23 | AI Support Indicators Dashboard | High | As a support analyst, I want to view tickets that have exceeded the SLA so that I can identify priority issues and act quickly to reduce delays in service. | 2 | 3 | Done | R28

---

## 🏃‍ DoR - Definition of Ready <a id="dor"></a>

- Tasks broken down from User Stories
- Design ready in Figma
- User Stories with Acceptance Criteria

---
  
## 🏆 DoD - Definition of Done <a id="dod"></a>

- User manual
- Complete code

---

## 📅 Sprint Schedule <a id="sprint"></a>

|      Sprint     |    Period     |
| :-------------: | :-----------: | 
| 🔖 **SPRINT 1** | 09/08 - 09/28 |
| 🔖 **SPRINT 2** | 10/06 - 10/26 | 
| 🔖 **SPRINT 3** | 11/03 - 11/23 |

---

## 🆕 Burndown <a id="burndown"></a>

### Sprint 1
![Imagem do WhatsApp de 2025-09-28 à(s) 17 33 42_8897514d](https://github.com/user-attachments/assets/0db5215f-15f6-473b-a0b2-4543b32f4947)

### Sprint 2
![Imagem do WhatsApp de 2025-10-29 à(s) 20 48 04_11da2c10](https://github.com/user-attachments/assets/d9aed1e8-0338-41dd-b28b-c37f86a0099f)

---

## 💻 Technologies <a id="technologies"></a>

<h4 align="center">
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D"/></a>
 <a href="https://www.mongodb.com/"><img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"></a>
 <a href="https://github.com/"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/></a>
 <a href="https://www.figma.com/"><img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white"/></a>
 <a href="https://pandas.pydata.org/"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"></a>
 <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"></a>
 <a href="https://facebook.github.io/prophet/"><img src="https://img.shields.io/badge/Prophet-6F4E37?style=for-the-badge&logo=prophet&logoColor=white"></a>
 <a href="https://github.com/flairNLP/flair/"><img src="https://img.shields.io/badge/Flair-FF6F00?style=for-the-badge&logo=flair&logoColor=white"></a>
</h4>

---

## 🎓 Team <a id="team"></a>

<div align="center">
  <table>
    <tr>
      <th>Member</th>
      <th>Role</th>
      <th>Github</th>
      <th>LinkedIn</th>
    </tr>
    <tr>
      <td>Cauan Barbaglio</td>
      <td>Product Owner</td>
      <td><a href="https://github.com/Cauanvmb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/cauan-barbaglio"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Vinícius Chaves</td>
      <td>Scrum Master</td>
      <td><a href="https://github.com/ChavesVini"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/vin%C3%ADcius-chaves-197353244"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Amanda Vannucci</td>
      <td>Developer</td>
      <td><a href="https://github.com/Amandavannuccic"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/amanda-vannucci"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Guilherme Wunderlich</td>
      <td>Developer</td>
      <td><a href="https://github.com/wunderlich-15"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/guilherme-wunderlich-aa56a2228"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Naiara Santos</td>
      <td>Developer</td>
      <td><a href="https://github.com/NaiaraSantos3"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/naiara-santos-73b83a186"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Raul Neto</td>
      <td>Developer</td>
      <td><a href="https://github.com/raulnt"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/raul-neto-b51b24157/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
  </table>
</div>

---

## ❗ More Information <a id="more_information"></a>
<p align="center">
  <a href="https://github.com/new-ge/LuminIA/wiki/Home">
    <img src="https://img.shields.io/badge/Wiki-Documentation-blue?style=for-the-badge&logo=read-the-docs&logoColor=white" alt="Wiki">
  </a>
</p>
For more information, please check the project Wiki, where you will find detailed documentation.
