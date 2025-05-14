# Kenneth N. Ngcobo

## Software & Electronics Engineer

📍 Johannesburg, South Africa  
📫 [nk.fuze@gmail.com](mailto:nk.fuze@gmail.com)
🔗 [LinkedIn](https://linkedin.com/in/kenneth-ngcobo-218b6746) | [GitHub](https://github.com/)

---

## About Me

I am an experienced **Software and Electronics Engineer** with a strong track record in full-stack web development and embedded systems. I specialize in building scalable web applications and consulting in the **LED lighting industry**, offering complete lifecycle services from concept to production.

With a passion for innovation and teaching, I also design and coach software development courses, fostering industry-aligned, future-ready skills.

---

## Skills

### Software & Web Development

<!-- `JavaScript`, `TypeScript`, `React`, `Next.js`, `Vue`, `Nuxt`, `Node.js`, `RESTful API`, `GraphQL`, `SQL/NoSQL`, `User Auth`, `Git`, `HTML`, `CSS`, `Tailwind CSS`, `Bootstrap` -->

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Vue](https://img.shields.io/badge/Vue.js-42b883?style=for-the-badge&logo=vue.js&logoColor=white)
![Nuxt](https://img.shields.io/badge/Nuxt.js-00DC82?style=for-the-badge&logo=nuxt.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![REST API](https://img.shields.io/badge/RESTful%20API-4B5563?style=for-the-badge&logo=fastapi&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
![SQL/NoSQL](https://img.shields.io/badge/SQL%20%2F%20NoSQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![User Auth](https://img.shields.io/badge/User%20Auth-4B5563?style=for-the-badge&logo=passbolt&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

### Embedded Systems

<!-- `C`, `C++`, `Python` -->

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### PCB Design & Electronics

<!-- `Altium`, `KiCad`, `EagleCAD` -->

![Altium](https://img.shields.io/badge/Altium%20Designer-000000?style=for-the-badge&logo=altiumdesigner&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB6?style=for-the-badge&logo=kicad&logoColor=white)
![EagleCAD](https://img.shields.io/badge/EagleCAD-CB2026?style=for-the-badge&logo=autodesk&logoColor=white)

---

## Projects

### Inventory and Job Management System

I developed a comprehensive **Inventory and Job Management System** using **Vue.js**, **Node.js**, and **MySQL**, designed to streamline component tracking, job kitting, and procurement processes. The system supports **bulk importing of component data** from existing Excel records, storing details such as **quantity, price, and supplier information** in a structured MySQL database.

#### Key Features

- **Real-time search with auto-suggestions** on the front end for quick component lookup.
- **BOM (Bill of Materials) uploads**, which dynamically deduct components from stock when assigned to jobs.
- **Job kitting integration** with barcode scanning:
  - Components are scanned via a scanner connected to a **Raspberry Pi**.
  - The scanner communicates with the system using **WebSockets**, enabling real-time stock updates.
- **Low stock alerts**, which automatically notify buyers when components fall below threshold levels.
- **Supplier purchase order (PO) generation**, with tracking of **expected delivery dates (ETAs)**.
- **Job ETA estimation**, factoring in missing components, their POs, and ETAs to provide accurate forecasting.

This system significantly improved operational efficiency, enhanced inventory accuracy, and optimized procurement and production planning workflows.

![Vue.js](https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=for-the-badge&logo=raspberry-pi&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

---

### QuoteLink – SFA-to-Sage Integration Bridge

I developed **QuoteLink**, a middleware system that seamlessly integrates the company’s quoting platform (**SFA**) with its ERP system (**Sage**) to eliminate redundant data entry, reduce human error, and accelerate sales order processing. The platform was built with **React**, **Node.js**, **Microsoft SQL Server**, **SMTP email services**, and secured with **user authentication**.

#### Problem

SFA enabled users to easily build custom lighting product quotes by selecting categories, wattages, beam angles, and other options. It generated **custom item codes** and calculated prices based on selected configurations. However, users then had to **manually check Sage** for existing codes or create new ones, and **manually re-enter** item details to generate a sales order — a time-consuming and error-prone process, especially for large quotes.

#### Solution & Key Features

- **Quote import**:

  - User enters the **SFA quote number** into QuoteLink.
  - The system retrieves all quote data directly from the **SFA database**.

- **Item code validation**:

  - Automatically checks if **generated item codes** exist in **Sage**.
  - Highlights any **missing codes**, which can be requested with a single click.
  - Sends a **notification to the responsible team** to create the missing codes.

- **Automated SO creation**:

  - Once all codes are confirmed, the user can generate a **Sales Order (SO)** in Sage with:
    - Correct item codes
    - Quantities and prices
    - Customer details
  - The **production team is notified** of the new SO for scheduling.

- **Error elimination**:
  - Fully removes the need to **retype or manually transfer** quote information into Sage.
  - Reduces processing time and improves accuracy in order fulfillment.

QuoteLink became a critical link in the company’s sales-to-production pipeline, improving efficiency, accuracy, and internal coordination across quoting, ERP, and manufacturing teams.

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Microsoft SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![SMTP](https://img.shields.io/badge/SMTP%20Email-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white)
![Authentication](https://img.shields.io/badge/User%20Auth-4B5563?style=for-the-badge&logo=passbolt&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

---

### QCTrack – Digital Quality Control and Non-Conformance System

I developed **QCTrack**, a digital quality control system tailored for a lighting manufacturing company to **log, manage, and analyze product non-conformance issues**, whether identified internally or returned from the field. The platform streamlined issue tracking, accountability, and root cause analysis, significantly improving traceability and process improvement efforts.

#### Key Features

- **Issue logging interface** for relevant staff to report non-conformances:

  - Attach **images** and provide detailed **descriptions**.
  - Select from a predefined list of **common fault categories** for consistent classification and future analysis.
  - Identify the **responsible department** (e.g., Technical, Mechanical Design, Production).

- **Automated email notifications** sent to the assigned individuals within the responsible department, including fault details and images.

- **Root cause analysis workflow**:

  - Responsible parties provide **cause investigation**, **preventative measures**, and **cost tracking** (e.g., replacement components).
  - Issues can be attributed to **categories** such as _supplier error_ or _production procedure fault_.
  - If supplier-related, their details are logged for follow-up.

- **Issue closure validation** ensures that all required fields are completed before an issue can be marked resolved.

- **Auto-generated QC reports**:

  - Upon closure, a **PDF report** is automatically created and emailed to the original reporter.
  - Includes all relevant data, including **client information** for traceability and customer communication.

- **Interactive analytics dashboard**:
  - Filter and visualize data to identify trends by **product**, **fault type**, or **supplier**.
  - Interactive bar charts allow users to click on a product or category to view associated issues.
  - Used actively in **QC meetings** and **ISO audits** to demonstrate issue resolution processes and trend tracking.

Built with a stack including **Nuxt.js**, **Node.js**, **MySQL**, and an integrated **SMTP email service**, QCTrack became a core part of the company's quality assurance and continuous improvement strategy.

![Nuxt.js](https://img.shields.io/badge/Nuxt.js-00C58E?style=for-the-badge&logo=nuxt.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white)
![SMTP Email](https://img.shields.io/badge/SMTP%20Email-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

---

### LumaTest – Internal Lab Scheduling and Reporting System

I developed **LumaTest**, a centralized lab scheduling and reporting system for a lighting manufacturing company with in-house **photometric**, **thermal**, and **IP testing** labs. The platform was built with **Nuxt.js**, **Node.js**, **MySQL**, and an integrated **SMTP email server** to streamline internal test requests, communication, and data access.

#### Key Features

- **Test booking interface** for internal stakeholders across departments to schedule tests with specific labs.
- Mandatory input of **fixture specifications** (e.g., wattage, length, CCT, CRI) to eliminate ambiguity about which variant was tested.
- Users specify **expected result dates** and **test priorities**, which are stored in the database and reflected on the lab's shared schedule.
- **Automated email notifications** to lab technicians upon new test requests.
- Lab technicians can:
  - Review their schedule and respond with a **revised promise date** if needed.
  - Trigger email updates to the requester with the new timeline.
- **Live lab schedules** visible to all relevant stakeholders, allowing departments to **negotiate and adjust priorities** collaboratively.
- Upon test completion:
  - Technicians upload **test reports** and mark tests as **pass/fail**.
  - The system sends an **automated email with the test report** to the requester.
- A centralized, **searchable and filterable test report archive** eliminates the need for manual file browsing across network folders.

LumaTest significantly improved internal coordination, reduced miscommunication, and streamlined access to historical testing data across the organization.

![Nuxt.js](https://img.shields.io/badge/Nuxt.js-00C58E?style=for-the-badge&logo=nuxt.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white)
![SMTP Email](https://img.shields.io/badge/SMTP%20Email-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
