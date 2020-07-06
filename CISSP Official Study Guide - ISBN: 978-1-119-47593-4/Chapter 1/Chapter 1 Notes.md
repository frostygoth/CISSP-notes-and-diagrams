# CISSP Chapter 1 Notes #

## *Important Information About Source Citation* ##

**Notes I've made from this chapter may be completely or partially extracted from the CISSP Official Study Guide ISBN: 978-1-119-47593-4. Although the format and additional thoughts may be my own, it is critical to give credit to the published document above. My notes are NOT exhaustive and I HIGHLY recommend that you purchase this book.**

**Should the publisher of the above document have any issues with the references to their source material above, please make a pull request and we can get the issue resolved.**

## Understand and Apply Concepts of Confidentiality, Integrity, and Availability ##

- The three major security principals are confidentiality, integrity, and availability.
	+ Confidentiality
		* Confidentiality is the concept of the measures used to ensure the protection of the secrecy of data, objects, or resources.
		* Attacks include capturing network traffic, stealing password files, social engineering, port scanning, shoulder surfing, eavesdropping, sniffing, escalation of privileges.
		* Counter measures include encryption, network traffic padding, strict access control, rigorous authentication procedures, data classification, and extensive personnel training.
		* Other concepts, conditions, and aspects of confidentiality include the following:
			- Sensitivity: Refers to the quality of information, which could cause harm or damage if disclosed.
			- Discretion: An act of decision where an operator can influence or control disclosure in order to minimize harm or damage.
			- Criticality: The level to which information is mission critical. The higher the criticality the more likely the need to maintain the confidentiality.
			- Concealment: The act of hiding something to prevent disclosure. Often concealment is viewed as a means of cover, obfuscation, or distraction.
			- Secrecy: The act of keeping something a secret or preventing the disclosure of information.
			- Privacy: This refers to keeping information confidential that is personally identifiable or that might cause harm, embarrassment, or disgrace to someone if revealed.
			- Seclusion: This involves storing something in an out-of-the-way location. This location can also provide strict access control.
			- Isolation: The act of keeping something separated from others. This can be used to prevent commingling of information or disclosure of information.

	+ Integrity
		* Integrity is the concept of protecting the reliability and correctness of data. Integrity protection prevents unauthorized alterations of data. 
		* Maintaining the data means that the object itself is not altered by unauthorized entities or unauthorized actions from authorized entities and the operating system and programming entities that manage and manipulate the object are not compromised.
		* Integrity can be examined from three perspectives:
			- Preventing unauthorized subjects from making modifications
			- Preventing authorized subjects from making unauthorized modifications, such as mistakes
			- Maintaining the internal and external consistency of objects a that their data is a correct and true reflection of the real world and any relationship with any child, peer, or parent object is valid, consistent, and verifiable.
		* Attacks include viruses, logic bombs, unauthorized access, errors in coding and applications, malicious modification, intentional replacement, and system back doors.
		* Counter measures include strict access control, rigorous authentication procedures, intrusion detection systems, object/data encryption, hash total verification, interface restrictions, input/function checks, and extensive personnel training.
		* Integrity is dependent on confidentiality.
		* Other concepts, conditions, and aspects of integrity include the following:
			- Accuracy: Being correct and precise
			- Truthfulness: Being a true reflection of reality
			- Authenticity: Being authentic or genuine
			- Validity: Being factually or logically sound
			- Non-repudiation: Not being able to deny having performed an action or activity or being able to verify the origin of a communication or event.
			- Accountability: Being responsible or obligated for actions and results.
			- Completeness: Having all needed and necessary components or parts.
			- Comprehensiveness: Being complete in scope; the full inclusion of all needed elements.
			
	+ Notes on non-repudiation.
		* Non-repudiation ensures that the subject of an activity or who caused an event cannot deny that the event occurred. It is made possible through identification, authentication, authorization, accountability, and auditing.
		* Non-repudiation can be established using digital certificates, session identifiers, transaction logs, and numerous other transaction and access control mechanisms.

	+ Availability
		* The purpose of availability is to ensure that authorized subjects are granted timely and uninterrupted access to objects. 
		* Availability includes efficient uninterrupted access to objects even during the implementation of active threats. It also includes the effective planning and implementing of supported infrastructure, which can insure that failure of a configuration item in the system does not unreasonably impact the availability of that system.
		* Threats to availability include device failure, software errors, and environmental issues such as heat and flooding. It also includes various attacks such as DoS attacks, object destruction, and communication interruptions.
		* Counter measures to risks include designing intermediary delivery systems properly, using access controls efficiently, monitoring performance and network traffic, using firewalls and routers to prevent DoS attacks, implementing redundancy for critical systems, and maintaining and testing backup systems. Security policies ,such as the business continuity plan, focus on the use of fault tolerance features at various levels of access/storage/security.
		* Availability depends on both integrity and confidentiality.
		* Other concepts, conditions, and aspects of availability include the following:
		* Usability: The state of being easy to use or learn or being able to be understood and controlled by a subject.
		* Accessibility: The assurance that the widest range of subjects can interact with a resource regardless of their capabilities or limitations.
		* Timeliness: Being prompt, on time, within a reasonable time frame, or providing low-latency response.  

- The AAA Services
	+ The AAA services stand for authentication, authorization, and accounting. However, there are more elements than just these three.
	+ The three elements of AAA services are as follows:
		* Identification: Claiming to be an identity when attempting to access a secured area or system.
		* Authentication: Proving you are that identity.
		* Authorization: Defining the permissions of a resource and object access for a specific identity.
		* Auditing: Recording a log of the events and activities related to the system and subjects.
		* Accounting: Reviewing log files to check for compliance and violations in order to hold subjects accountable for their actions.
	+ Typically AAA is referenced in relation to authentication systems (TACACS+, Kerberos, 802.11x), but it is actually a foundational concept for security. Missing any of these five elements can result in an incomplete security mechanism.
	+ The 5 AAA services have chained dependencies on each other. See below.
	+ Identification --> Authentication --> Authorization --> Auditing --> Accounting
	+ **Identification**
		* Examples of providing an identity can include typing a username, swiping a smart card, waving a proximity device, speaking a phrase, and positioning your face, hand or finger for a camera or scanning device among other things.
		* Without an identity, a system has no way to correlate an authentication factor with the subject. **Observer the relationship here**
		* I.T. systems track activity by identities, not the subjects themselves. This is why things like password sharing, and social engineering are such significant problems.
	+ **Authentication**
		* Authentication is the process of verifying or testing that the claimed identity is valid. It requires that the subject provides additional information that corresponds to the identity they are claiming. This additional information is known as the authentication factor and is used to verify the identity and is typically labeled as, or considered to be, private information.
	+ **Authorization**
		* The process of authorization ensures that the request activity or access to an object is possible given the rights and privileges assigned to the associated identity. In most cases the system evaluates an access control matrix that compares the subject, the object, and the intended activity.
		* Authorization is usually defined using one of the models of access control, such as *Discretionary Access Control*, *Mandatory Access Control*, or *Role Based Access Control*.
	+ **Auditing**
		* Auditing is the programmatic means by which a subject's actions are tracked and recorded for the purpose of holding the subject accountable for their actions. It is also the process by which unauthorized or abnormal activities are detected on a system.
		* Monitoring is part of what is needed for audits, and audit logs are part of a monitoring system, but the two terms have different meanings. Monitoring is a type of watching or oversight, while auditing is a recording of the information into a record of file. It is possible to monitor without auditing, but you can't audit without some form of monitoring.
	+ **Accountability**
		* Accountability is established by linking a human to the activities of an online identity through the security services and mechanisms of auditing, authorization, authentication, and identification.

- Protection Mechanisms that offer protection for CIA
	+ Layering
		* Layering, also known as defense in depth, is simply the use of multiple controls in a series. Note, not parallel. By layering consecutive controls you force a subject to be challenged multiple times, where a single failure causes them to fail. If you were to have multiple controls in parallel, then the subject would only need to pass one of the controls to succeed.
	+ Abstraction
		* Abstraction is used for efficiency. Similar elements are put into groups, classes, or roles that are assigned security controls, restrictions, or permissions as a collective. Think RBAC.
	+ Data Hiding
		* Data hiding prevents data from being discovered or accessed by a subject by positioning the data in a logical storage compartment that is not accessible or seen by the subject.
		* This is different from security through obscurity. Data hiding is the act of intentionally positioning data so that it is not viewable or accessible to an unauthorized subject, while security through obscurity is the idea of not informing the subject about an object being present and thus hoping that the subject will not discover the object.
	+ Encryption
		* Encryption is the art and science of hiding the meaning or intent of a communication from unintended recipients.
		
## Evaluate and Apply Security Governance Principals ##

- Overview
	+ **Security governance** is the collection of practices related to supporting, defining, and directing the security efforts of an organization. Security governance principals are often closely related to and often intertwined with **corporate governance** and **IT governance*.
	+ The common goal of governance is to maintain business processes while striving toward growth and resiliency.
	+ Security governance is the implementation of a security solution and a management method that are tightly connected.
- Alignment of Security Function to Business Strategy, Goals, Missions, and Objectives.
	+ Security management planning aligns the security functions to the strategy, goals, missions and objectives of the organization and ensures the proper creation, implementation, and enforcement of a security policy.
	+ One of the most effective ways to tackle security management planning is to use a top-down approach, where upper, or senior, management is responsible for initiating and defining policies for the organization.
	+ The security policy provides direction for all levels of the organization's hierarchy. It is the responsibility of middle management to flesh out the security policy into standards, baselines, guidelines, and procedures. The operational managers or security professionals must then implement the configuration prescribed in the security management documentation.
		* Security management is a responsibility of upper management, not of the IT staff, and is considered an issue of business operations rather than IT administration. The team or department responsible for security within the organization should be autonomous.
		* The information security team should be lead by a designated chief information security officer who must report directly to senior management. Placing the autonomy of the CISO and the CISO's team outside the typical hierarchical structure in an organization can improve security management across the entire organization. It will also help to avoid cross-department and internal political issues.
		* The best security plan is useless without approval from senior management since at the end of the day, the results of the security plan come back to them.
	+ A security management planning team should develop three types of plans.
		* Strategic Plan
			- A strategic plan is a long-term plan that is fairly stable. It defines the organization's security purpose and it helps to understand security function and align it to the goals, mission, and objectives of the organization. 
			- It's useful for about five years if it is maintained and updated annually.
			- A strategic plan serves as the planning horizon, with long-term goals and visions for the future being discussed.
			- A strategic plan should include a risk assessment.
		* Tactical Plan
			- The tactical plan is a midterm plan developed to provide more details on accomplishing the goals set forth in the strategic plan or can be crafted ad hoc based upon unexpected events.
			- A tactical plan is useful for about a year and also prescribes and schedules the tasks necessary to accomplish organizational goals.
			- Examples of tactical plans are project plans, acquisition plans, hiring plans, budget plans, maintenance plans, support plans and system development plans.
		* Operational Plan
			- An operational plan is a short-term, highly detailed plan based on the strategic and tactical plans.
			- It is valid or useful for only a short time and operational plans must be updated often to retain compliance with tactical plans.
			- Operational plans spell out how to accomplish the various goals of the organization. They include resource allotments, budgetary requirements, staffing assignments, scheduling, and step-by-step procedures. They also include details on how the implementation processes are in compliance with the organization's security policy. 
			- Examples of operational plans include training plans, system development plans, and product design plans. 
- Organizational Processes
	+ Storage Media should be removed and destroyed, because media sanitization techniques do not guarantee against data remnant recovery.
- Change Control/Management
	+ The goal of change management is to ensure that any change does not lead to reduced or compromised security. Change management is also responsible for making it possible to roll back any change to a previous secured state.
	+ Change management ensures that its goal is achieved by making sure all changes are subject to detailed documentation and auditing and thus able to be planned, reviewed, and scrutinized by management.
	+ The change control process of configuration or change management has several goals or requirements itself.
		* Implement changes in a monitored and orderly manner. Changes are always controlled.
		* A formalized testing process is included to verify that a change produces expected results.
		* All changes can be reversed (also known as backout or rollback plans/procedures).
		* Users are informed of changes before they occur to prevent loss of productivity.
		* The effects of changes are systematically analyzed to determine whether security or business processes are negatively affected.
		* The negative impact of changes on capabilities, functionality, and performance is minimized.
		* Changes are reviewed and approved by a Change Advisory Board.
		
# WIP #

## Chapter Terms ##

- Object: The passive element in a security relationship, such as files, computers, network connections, and applications. A subject acts upon or against an object.
- Subject: The active element in a security relationship, such as users, programs, and computers. A subject acts upon or against an object.
- Access Control: The term used to refer to the management of the relationship between subjects and objects.
- Network Traffic Padding: A counter measure meant to protect the confidentiality of a network by inserting dummy traffic into the network to confuse a threat by changing the pattern of network flow.
- Access/storage/security: Represents various points in a system at which you can introduce fault tolerance features.
- Operational Technology Systems: A system that contains hardware and software that detects or causes a change, through the direct monitoring and/or control of industrial equipment, assets, processes and events.
- Programmable Logic Controllers: An industrial digital computer which has been ruggedized and adapted for the control of manufacturing processes, such as assembly lines, or robotic devices, or any activity that requires high reliability, ease of programming and process fault diagnosis.
- Supervisory Control and Data Acquisition: A control system architecture comprising of computers, networked data communications and graphical user interfaces for high-level process supervisory management. It also comprising other peripheral devices like programmable logic controllers to interface with process plants or machinery.
- Manufacturing Execution Systems: These are computerized systems used in manufacturing to track and document the transformation of raw materials to finished goods. These systems provide information that helps manufacturing decision makers understand how current conditions on the plant floor can be optimized to improve production output.
- Access Control Matrix: An abstract, formal security model of protection state in computer systems, that characterizes the rights of each subject with respect to every object in the system.
- Discretionary Access Control: A type of security access control that grants or restricts object access via an access policy determined by an object's owner group and/or subjects.
- Mandatory Access Control: A type of security access control by which the operating system constrains the ability of a subject to access or generally perform some sort of operation on an object.
- Role Based Access Control: A type of security access control mechanism defined around roles and privileges. Role Based Access Control can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions thanks to its use of role-permissions, such as user specific and group specific role-permissions.
- Security Policy: For an organization, this addresses the constraints on behavior of its members as well as constraints imposed on adversaries in order to establish a definition of what it means to be secure for the system.
- Business Case: A documented argument or stated position in order to define a need to make a decision or take some form of action.