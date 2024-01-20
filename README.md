# Securing-a-Cloud-based-Healthcare-Application-in-AWS

The Aim of this project is to assess the security vulnerabilities in a healthcare company's cloud infrastructure. The application is designed to store and manage sensitive patient data, including medical records, personal information, and billing details. The task is to ensure the confidentiality, integrity, and availability of the application and its data, as well as to identify and mitigate potential security risks. The project will involve various aspects of cloud security, including identity and access management, data encryption, network security, and vulnerability management.

The company relies on the cloud to store and manage sensitive patient data, conduct telemedicine consultations, and host critical healthcare applications. However, due to various security oversights and misconfigurations, the infrastructure is highly vulnerable to potential attacks. The task is to identify and exploit these vulnerabilities to highlight the risks associated with the insecure cloud infrastructure and provide recommendations for remediation. 

The application stack consists of the following components:

**Web servers**: These serve the frontend of the website and handle user requests.
**Application servers**: These handle the business logic and process user requests.
**Database servers**: These store product information, user details, and medical history.

The cloudformation in the following github repository was used: https://github.com/edaviage/medcircle-midterm

**Infrastructure Details:**
 
Cloud Provider: The healthcare company uses a popular cloud service provider (e.g., AWS, Azure, Google Cloud) for hosting its infrastructure.
Data Storage: Patient records, medical images, and other sensitive healthcare data are stored in cloud-based databases and file storage systems.
Virtual Machines (VMs): The company utilizes VMs for hosting healthcare applications and databases.
Network Configuration: The cloud infrastructure has several virtual networks and subnets for different departments and services within the company.
Identity and Access Management (IAM): The healthcare company employs IAM policies and access controls for managing user access to cloud resources.
The IT department requires full access to both frontend and backend instances for management purposes.
All instances should be automatically assigned public and private IP addresses where necessary
The VPC should be designed to accommodate future growth and scalability.
 

**Insecure Infrastructure Issues:**

Weak Access Controls: The IAM policies and access controls have been misconfigured, resulting in excessive permissions and unauthorized access to critical resources. IAM policies are available in the Midterm section under the Modules tab.
Unencrypted Data: Sensitive patient data stored in databases and file storage systems is not adequately encrypted, making it susceptible to unauthorized access.
Vulnerable Virtual Machines: The VMs running healthcare applications and databases have outdated software and unpatched vulnerabilities.
Inadequate Network Security: Network security groups and firewall rules have not been properly configured, allowing unrestricted access to sensitive resources.
Lack of Logging and Monitoring: The infrastructure lacks robust logging and monitoring mechanisms, making it difficult to detect and respond to security incidents.
Insufficient Disaster Recovery: There is no comprehensive backup and disaster recovery plan in place, making the infrastructure susceptible to data loss and extended downtime.
 

**Project Tasks:** 

Assess the IAM policies and access controls, identifying vulnerabilities and excessive permissions.
Exploit weak access controls to gain unauthorized access to critical resources and demonstrate the potential impact.
Perform a security assessment of the databases and file storage systems, highlighting the risks associated with unencrypted data.
Exploit vulnerabilities in the virtual machines to gain unauthorized access or demonstrate the potential impact of an attack.
Evaluate the network security configuration, identifying vulnerabilities and demonstrating the consequences of unrestricted access.
Analyze the logging and monitoring capabilities, identifying weaknesses and proposing improvements for detecting and responding to security incidents.
Assess the disaster recovery plan, highlighting the risks of data loss and extended downtime due to insufficient backup mechanisms.

After completing the above tasks, documention of the following reports were made:

Vulnerability assessment report, detailing the identified weaknesses and their potential impact on the healthcare company's cloud infrastructure.
Data security assessment report, highlighting the risks associated with unencrypted patient data and providing recommendations for secure data storage and encryption.
Virtual machine vulnerability assessment report, outlining the vulnerabilities in the VMs and recommending patching and vulnerability management measures.
Network security assessment report, identifying vulnerabilities in network security and proposing improvements for secure access control..
Disaster recovery assessment report, highlighting the risks of data loss and extended downtime and proposing a comprehensive backup and disaster recovery plan.

Based on the above analysis reports made, a high level overview of the infrastructure changes were made. Documentation on the services and methodologies that was intended to employ to mitigate the security risk that have been identified from various assessment reports are given. It also includes architectural diagrams that provides a high level overview of the proposed architecture. These diagrams includes accurate dataflows that cover three scenarios. 

The first scenario is from the patient's point of view. The patients will access the portal from personal devices and will participate in telemedicine consultations as well as accessing test results, scheduling appointments and general inquiries.
The second scenario is from the care providers point of view. They will have access to all patients data as well as the ability to send and receive messages from third parties including hospitals
The third scenario is from the IT support point of view. The IT team may have several roles including end user support, DBAs, system administrators and super admins.
Your technical overview and diagrams should cover the basic application and additional cloud services and tools that will be used to mitigate the identified risks. The level of detail of your diagram should closely resemble your technical overview.
