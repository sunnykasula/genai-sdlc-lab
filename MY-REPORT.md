![GenI-Banner](https://github.com/genilab-fau/genial-fau.github.io/blob/8f1a2d3523f879e1082918c7bba19553cb6e7212/images/geni-lab-banner.png?raw=true)

# {How can prompt engineering techniques be applied to automate the requirement analysis process in the Software Development Lifecycle (SDLC)?
}

1-liner description of your project

<!-- WHEN APPLICABLE, REMOVE THE COMMENT MARK AND COMPLETE
This is a response to the Assignment part of the COURSE.
-->

* Authors: Sai Vardhan Reddy Kasula  
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

  
# Research Question 
How can **large language models (LLMs)** and **prompt engineering techniques** be leveraged to automate **requirement analysis** within the **Software Development Lifecycle (SDLC)**, improving accuracy, efficiency, and reducing ambiguity in software engineering?

---
Requirement engineering is a **critical phase** in the **Software Development Lifecycle (SDLC)**, defining system functionalities and constraints before development begins. However, traditional methods of requirement analysis often suffer from:  

1. **Ambiguity & Inconsistency** – Requirements are often vague or misinterpreted, leading to software defects.  
2. **Time-Intensive Manual Processing** – Human analysts must validate, structure, and refine requirements.  
3. **Scalability Challenges** – Large projects require extensive requirement documentation and validation.  

This research explores how **AI-driven prompt engineering techniques**—such as **Zero-shot, Few-shot, Chain-of-Thought (CoT), Meta Prompting, and Template-based prompting**—can **automate** and **enhance** requirement analysis by leveraging **LLMs** like **GPT-3.5-turbo**.

## Arguments

#### What is already known about this topic
### **What is already known about this topic**  
- **AI-driven NLP models** have demonstrated significant advancements in **natural language understanding**, allowing automated interpretation of software requirements.  
- **Prompt engineering** has emerged as a method to fine-tune LLM responses based on structured input formatting.  
- AI models have been successfully applied in **code generation, test case generation, and requirement validation**, but **automated requirement extraction and refinement remain largely unexplored**.  

### **What this research is exploring**  
- Employing **prompt engineering techniques** to **extract, analyze, and refine** software requirements.  
- Developing **a structured methodology** for generating **functional and non-functional requirements** using AI.  
- Exploring how **LLMs** can **reduce ambiguity** in software specifications and improve **requirement validation**.  

### **Implications for practice**  
- **Improved accuracy** – AI-driven requirement analysis reduces human error.  
- **Optimized SDLC processes** – Automation enhances efficiency in software engineering workflows.  
- **Better standardization** – Structured prompt-based extraction ensures consistent requirement documentation.  

---


# Research Method
### **1. Experimental Setup**  
The study involved **iterative experimentation** with various **prompt engineering techniques** to analyze how LLMs process software requirements. The methodology involved:  

- **Dataset:** Manually curated requirements from real-world software projects.  
- **LLM Model:** OpenAI’s **GPT-3.5-turbo API**.  
- **Testing Scenarios:** Applied on **banking, IoT, fitness, SaaS, and e-commerce** domains.  
- **Evaluation Metrics:** **Accuracy, Consistency, and Context Awareness** of responses.

- ### **2. Prompt Engineering Techniques Evaluated**  

| **Prompting Technique** | **Objective** | **Findings** |
|-------------------------|--------------|-------------|
| **Zero-Shot Prompting** | Understanding LLM's ability to infer requirements without context | Generated generic but logically structured outputs. Lacked domain-specific depth. |
| **Few-Shot Prompting** | Providing example-based learning for improved response accuracy | Increased specificity and coherence in structured requirement extraction. |
| **Chain-of-Thought (CoT) Prompting** | Encouraging step-by-step breakdown of complex queries | Improved interpretability and logical flow in requirement refinement. |
| **Meta Prompting** | Enhancing clarity by rephrasing ambiguous queries | Significant reduction in ambiguity. Useful in refining unclear requirements. |
| **Template-Based Prompting** | Enforcing structured response formats | Ensured consistency in requirement extraction across domains. |

---

# Results

### **1. Case Study: Requirement Analysis for an Online Banking System**  
Experiment 1:
Prompt: Analyze and list the key functional and non-functional requirements for an online banking system.
Response:
Key Functional Requirements:
1. User Registration: Users should be able to create an account with the online banking system.
2. Account Management: Users should be able to view account balances, transaction history, and manage
their accounts online.
3. Fund Transfer: Users should be able to transfer funds between their own accounts or to other accounts
within the same bank or to external accounts.
4. Bill Payment: Users should be able to pay bills online, including utilities, credit cards, loans, and other
services.
5. Deposit and Withdrawal: Users should be able to deposit money into their accounts through online
transfers or mobile check deposit, as well as withdraw funds through online transfers or ATM withdrawals.
6. Alerts and Notifications: Users should receive notifications for account activities, such as low balance
alerts, payment reminders, and transaction confirmations.
7. Secure Messaging: Users should be able to communicate securely with the bank for inquiries, issue
resolution, and support.
8. Account Statement Generation: Users should be able to view and download account statements for a
specified period.
9. Loan Management: Users should be able to apply for loans, view loan details, and make loan payments
online.
10. Investment Management: Users should be able to view investment portfolios, buy/sell securities, and
manage investment accounts online.

#### **Functional Requirements (Extracted via Prompting)**  
- **User Registration:** Secure authentication with multi-factor verification.  
- **Fund Transfer:** Real-time and scheduled transactions with fraud detection.  
- **Bill Payment:** Integrated with external billing providers.  
- **Secure Messaging:** Encrypted communication between users and the bank.  

#### **Non-Functional Requirements (Identified through AI-Driven Analysis)**  
- **Scalability:** Support for high concurrent user load.  
- **Security:** AES-256 encryption, compliance with banking standards (PCI-DSS).  
- **Reliability:** 99.99% uptime with automatic failover mechanisms.  

#### **Ambiguity Resolution Example**  
**Requirement:** _"The system must support real-time transaction processing."_  
**Challenges Identified:**  
- **Definition of "real-time"** – Immediate vs. batch processing?  
- **Performance benchmarks** – Maximum allowable processing delay?  
- **Failure handling mechanisms** – What happens if a transaction fails?  

By applying **Chain-of-Thought (CoT) Prompting**, we extracted detailed sub-requirements to clarify ambiguities.

  


# Further research
### **2. Case Study:  

Experiment 2:
Prompt: For the requirement: 'The system must support real-time transaction processing', identify any
ambiguities and list potential edge cases.
Response:
Ambiguities:
1. What is the definition of "real-time" in this context? Does it mean immediate processing or processing
within a specific time frame?
2. What types of transactions are considered for real-time processing? Are there specific criteria or
conditions for a transaction to be processed in real-time?
3. Is there a specific performance benchmark or latency requirement for processing transactions in realtime?
4. Are there any constraints or limitations in terms of the volume or frequency of transactions that can be
processed in real-time?
Potential edge cases:
1. Handling concurrent real-time transactions: How will the system manage and prioritize multiple real-time
transactions happening simultaneously?
2. Handling transaction failures: What happens if a real-time transaction processing fails or encounters an
error? How will the system ensure data integrity and consistency?
3. Scalability: How will the system scale to support an increasing number of real-time transactions without
compromising performance or reliability?
4. Network latency: How will the system account for network delays or interruptions that may impact the realtime processing of transactions?
5. Data synchronization: How will the system ensure that data is synchronized in real-time across different
components or systems involved in transaction processing?
6. Security and compliance: How will the system maintain security and compliance requirements while
processing transactions in real-time?
---------------------------------------------------

Experiment 3:
Prompt: Provide a detailed breakdown of requirements for a mobile fitness tracking application, including
functional requirements, non-functional requirements, and potential user scenarios.
Response:
Sure! Here is a breakdown of requirements for a mobile fitness tracking application:
### Functional Requirements:
1. **User Registration and Profile Management:**
 - Users should be able to create an account and set up their profiles with personal information, fitness
goals, and preferences.
 - Users should be able to log in securely with authentication mechanisms.
2. **Activity Tracking:**
 - Users should be able to track various fitness activities such as running, cycling, walking, and workouts.
 - The app should allow users to record distance, duration, pace, calories burned, and route maps for each
activity.
3. **Goal Setting and Monitoring:**
 - Users should be able to set fitness goals such as daily step count, calorie intake, distance to run, etc.
 - The app should provide visual progress tracking towards goals and send notifications for goal
achievements.
4. **Workout Plans and Exercises:**
 - Users should have access to predefined workout plans and exercises for different fitness levels and goals.
 - The app should allow users to create custom workout plans and add new exercises.
5. **Social Features:**
 - Users should be able to connect with friends, share their activities, and compete in challenges.
 - The app should have social features like commenting, liking, and following other users.
6. **Integration with Wearable Devices:**
 - The app should be able to sync data with popular fitness trackers and smartwatches for accurate activity
tracking.
 -
------------------------------------------------------------
Experiment 4:
Prompt: Discuss the critical non-functional requirements that must be considered when designing a cloudbased SaaS platform, including performance, security, and scalability.
Response:
When designing a cloud-based Software as a Service (SaaS) platform, several critical non-functional
requirements need to be considered to ensure the platform's success. These requirements typically fall
under categories such as performance, security, and scalability. Let's discuss each of these in detail:
1. Performance:
 - **Response Time**: Users expect fast response times when interacting with a SaaS platform. Ensuring low
latency and quick loading times is crucial to providing a seamless user experience.
 - **Throughput**: The platform should be able to handle a high volume of concurrent users and
transactions without performance degradation.
 - **Resource Utilization**: Efficient utilization of resources such as CPU, memory, and storage is essential
to optimize performance and cost-effectiveness.
 - **Availability**: The platform should be highly available to minimize downtime and ensure continuous
access for users.
2. Security:
 - **Data Encryption**: Data transmitted between the user and the platform should be encrypted to prevent
unauthorized access and ensure data privacy.
 - **Authentication and Authorization**: Implement secure authentication mechanisms to verify user
identities and control access to resources based on user roles and permissions.
 - **Data Protection**: Implement robust data protection measures, including regular backups, disaster
recovery plans, and data retention policies.
 - **Compliance**: Ensure compliance with industry regulations and standards such as GDPR, HIPAA, or
PCI DSS to protect user data and maintain trust.
3. Scalability:
 - **Horizontal Scalability**: The platform should be
------------------------------------------------------------
Experiment 5:
Prompt: Explain how prompt engineering techniques can be used to identify ambiguous requirements in a
software project. Provide examples.
Response:
Prompt engineering techniques can be effectively used to identify ambiguous requirements in a software
project by breaking down and analyzing requirements in a structured and systematic manner. Here are some
techniques and examples of how they can help identify ambiguous requirements:
1. **Questioning and Clarifying**: Prompt engineering involves asking targeted questions to clarify and
elaborate on requirements. By asking questions such as "Can you provide more details on this requirement?"
or "What exactly do you mean by this term?", ambiguity in requirements can be uncovered. For example, if a
requirement states "The system should be user-friendly", prompt engineering techniques can prompt
questions like "What specific features or characteristics make a system user-friendly?" to clarify the
requirement.
2. **Scenario-based Analysis**: Creating scenarios based on requirements can help uncover ambiguities by
simulating how a user would interact with the system. For instance, if a requirement states "The system
should display relevant information", prompt engineering can prompt the creation of scenarios like "What
specific information is considered relevant in different contexts?" to identify potential ambiguities.
3. **Prototyping**: Building prototypes or mockups based on requirements can help visualize the expected
system behavior and functionality. By using prompt engineering techniques to review the prototype with
stakeholders, ambiguities in requirements can be identified early on. For example, if a requirement states
"The system should allow users to easily navigate between pages", a prototype can prompt questions like
"What navigation elements should be included to ensure ease of use?" to uncover ambiguities.
4. **Trace
------------------------------------------------------------
Experiment 6:
Prompt: Perform a chain-of-thought analysis for the requirement: 'The app must allow users to securely
upload and share photos.' Outline the functional steps, security considerations, and potential improvements.
Response:
Chain-of-Thought Analysis for the Requirement:
Functional Steps:
1. User Authentication: The app should require users to log in with a secure username and password to
access the upload and sharing features.
2. Upload Photo: Users should be able to select photos from their device and upload them securely to the
app's server.
3. Secure Storage: The uploaded photos should be stored securely on the server to prevent unauthorized
access.
4. Sharing Options: Users should have the ability to share uploaded photos with selected individuals or
groups within the app.
5. Access Control: The app should allow users to set permissions for who can view and download shared
photos.
Security Considerations:
1. Encryption: All communication between the app and the server should be encrypted to protect user data
from interception.
2. Data Protection: Implement secure storage practices to prevent data breaches and unauthorized access to
uploaded photos.
3. Access Controls: Use role-based access control mechanisms to ensure that only authorized users can
upload, view, and share photos.
4. Secure Authentication: Implement multi-factor authentication to enhance the security of user accounts
and prevent unauthorized access.
5. Regular Security Audits: Conduct regular security audits to identify and address any vulnerabilities in the
app's infrastructure.
Potential Improvements:
1. End-to-End Encryption: Implement end-to-end encryption for shared photos to ensure that only the
intended recipients can view them.
2. Two-Factor Authentication: Enhance security by implementing two-factor authentication for user
accounts.
3. Secure Sharing Options
------------------------------------------------------------
Experiment 7:
Prompt: List and explain the security requirements that should be implemented for an e-commerce website
to protect user data and prevent fraud.
Response:
1. Secure Socket Layer (SSL) Encryption: Implement SSL encryption to secure data transmission between the
user's browser and the e-commerce website. This helps prevent interception of sensitive information such as
credit card details.
2. Secure Payment Gateway: Use a reputable and secure payment gateway to process online transactions.
This ensures that financial transactions are encrypted and secure, reducing the risk of fraud.
3. Strong Password Policies: Enforce strong password policies for user accounts, including requirements for
complex passwords and regular password changes. This helps prevent unauthorized access to user
accounts.
4. Two-Factor Authentication (2FA): Implement two-factor authentication for user logins to add an extra layer
of security. This requires users to provide a second form of verification, such as a code sent to their mobile
device, in addition to their password.
5. Regular Security Audits and Penetration Testing: Conduct regular security audits and penetration testing to
identify and address vulnerabilities in the e-commerce website. This helps ensure that the website is secure
against potential threats.
6. Data Encryption: Encrypt sensitive user data stored in the database to protect it from unauthorized access.
This includes encrypting customer information such as credit card details, addresses, and personal
information.
7. Secure File Uploads: Implement measures to secure file uploads on the website to prevent malicious files
from being uploaded and executed on the server. This helps protect against potential security threats.
8. Fraud Detection and Prevention: Utilize fraud detection tools and services to monitor transactions for
suspicious activities and patterns
------------------------------------------------------------
Experiment 8:
Prompt: Analyze the requirement: 'The system should automatically scale to handle variable loads.' Identify
both the functional and non-functional requirements and any potential challenges.
Response:
Functional Requirement:
- The system should be able to automatically adjust its resources to accommodate varying levels of incoming
loads.
Non-functional Requirements:
- The system should respond to changes in load within a reasonable timeframe.
- The scaling process should not disrupt the ongoing operations of the system.
- The system should be able to scale both horizontally (adding more instances) and vertically (increasing
resources of existing instances).
- The scaling process should be cost-effective and efficient.
- The system should be able to monitor and predict load changes accurately to scale proactively.
- The system should maintain performance levels even during scaling operations.
Challenges:
1. Predicting load changes accurately: One challenge is accurately predicting when and by how much the
load will change to scale the system effectively.
2. Cost management: Scaling up resources can incur additional costs. Balancing the need for scalability with
cost efficiency is crucial.
3. Handling concurrent scaling operations: Ensuring that scaling operations do not interfere with each other
and impact system performance.
4. Monitoring and alerting: Implementing robust monitoring mechanisms to detect load changes and trigger
scaling actions in a timely manner.
5. Compatibility with existing infrastructure: Ensuring that the system's scaling mechanisms integrate
seamlessly with the existing infrastructure and technologies in use.
------------------------------------------------------------
Experiment 9:
Prompt: Generate a prioritized list of key requirements for a modern project management tool, including
features, usability, integration, and performance metrics.
Response:
Sure, here is a prioritized list of key requirements for a modern project management tool:
1. **User Interface (UI) and User Experience (UX)**
 - Intuitive and easy-to-use interface for all types of users
 - Customizable dashboard and project views
 - Drag-and-drop functionality for tasks and timelines
 - Mobile responsiveness for on-the-go access
2. **Task Management**
 - Ability to create, assign, and prioritize tasks
 - Task dependencies and subtask support
 - Task progress tracking and notifications
 - Kanban board or Gantt chart for visual task management
3. **Collaboration and Communication**
 - Real-time chat and messaging for team communication
 - File sharing and version control
 - Commenting and feedback features on tasks and projects
 - Integration with popular communication tools like Slack or Microsoft Teams
4. **Integration**
 - Integration with popular third-party tools like Google Drive, Dropbox, and Microsoft Office
 - API support for custom integrations with other software
 - Synchronization with calendar applications like Google Calendar or Outlook
5. **Reporting and Analytics**
 - Customizable reports on project progress, team performance, and resource allocation
 - Visual analytics and data visualization tools
 - Export options for sharing reports with stakeholders
6. **Security and Permissions**
 - Role-based access control for different user roles
 - Data encryption and secure data storage
 - Two
------------------------------------------------------------
Experiment 10:
Prompt: Using prompt engineering, provide an automated requirement analysis for a smart home IoT system.
Identify functional requirements, potential security risks, and scalability considerations.
Response:
**Automated Requirement Analysis for Smart Home IoT System**
**Functional Requirements:**
1. **Remote Monitoring and Control:** Users should be able to remotely monitor and control various devices
in their smart home such as lights, thermostats, locks, and security cameras.
2. **Automation:** The system should support automation of routine tasks based on predefined schedules,
triggers, or user preferences.
3. **Energy Management:** The system should provide energy usage monitoring and optimization features to
help users reduce energy consumption.
4. **Security Monitoring:** Integration with security sensors and alarms for real-time monitoring and alerts in
case of any security breaches.
5. **User Authentication and Access Control:** Implement robust user authentication mechanisms and
access control to ensure only authorized users can access and control the smart home devices.
6. **Interoperability:** Support for interoperability with various IoT devices and protocols to ensure seamless
integration and communication between different devices.
7. **Data Logging and Analytics:** Capture and analyze data from smart home devices to provide insights
and improve overall system performance and user experience.
**Potential Security Risks:**
1. **Unauthorized Access:** Hackers gaining unauthorized access to the system and controlling smart home
devices.
2. **Data Privacy:** Breaches in data privacy leading to exposure of sensitive user information.
3. **Device Vulnerabilities:** Exploitation of vulnerabilities in IoT devices leading to security breaches.
4. **Network Security:** Weak network security measures leading to interception of communication
between devices.
5. **Physical Security

---

## **Discussion & Lessons Learned**  

### **Key Takeaways**  
1. **Prompt engineering significantly enhances requirement extraction accuracy** – LLMs can effectively translate unstructured inputs into structured requirement breakdowns.  
2. **Chain-of-Thought (CoT) and Meta Prompting are particularly effective** – These techniques help in **clarifying ambiguities and refining vague software requirements**.  
3. **Automating requirement analysis reduces manual effort** – AI-driven requirement extraction can streamline SDLC documentation and validation processes.  
4. **Challenges remain in model reliability and scalability** – Some LLM outputs **require human validation** to ensure correctness in complex scenarios.  

### **Future Research Directions**  
- **Fine-tuning domain-specific LLMs** for **software engineering applications**.  
- **Integration of LLMs with Agile workflows** for **real-time requirement tracking**.  
- **Exploring reinforcement learning** to further refine requirement extraction accuracy.  

---

## **Conclusion**  
The project goal which aimed to investigate prompt engineering methods for automating requirement
analysis has been successfully met. After overcoming initial setup challenges of Ollama I moved to
GPT‑3.5‑turbo and performed experimental tests using zero-shot, few-shot, chain-of-thought, meta, and
template-based prompts. The different techniques each demonstrated unique ways to structure inquiries
and direct the model to produce more precise or understandable answers.
The documentation of these experiments revealed that prompt engineering extends beyond creating superior
questions to systematically directing a model's thought process and achieving consistency while enabling
the possibility of automating intricate tasks such as requirement analysis. This research demonstrates that
well-designed prompts enable extraction of detailed and dependable data from large language models which
then can be implemented in practical SDLC applications.
---
