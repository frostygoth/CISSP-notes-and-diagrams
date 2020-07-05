#CISSP Chapter 1 Notes#

##*Important Information About Source Citation*##

**Notes I've made from this chapter may be completely or partially extracted from the CISSP Official Study Guide ISBN: 978-1-119-47593-4. Although the format and additional thoughts may be my own, it is critical to give credit to the published document above. My notes are NOT exhaustive and I HIGHLY recommend that you purchase this book.**

**Should the publisher of the above document have any issues with the references to their source material above, please make a pull request and we can get the issue resolved.**

##Understand and Apply Concepts of Confidentiality, Integrity, and Availability##

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

##Chapter Terms##

- Object: The passive element in a security relationship, such as files, computers, network connections, and applications. A subject acts upon or against an object.
- Subject: The active element in a security relationship, such as users, programs, and computers. A subject acts upon or against an object.
- Access Control: The term used to refer to the management of the relationship between subjects and objects.
- Network Traffic Padding: A counter measure meant to protect the confidentiality of a network by inserting dummy traffic into the network to confuse a threat by changing the pattern of network flow.
- Access/storage/security: Represents various points in a system at which you can introduce fault tolerance features.
- Operational Technology Systems: A system that contains hardware and software that detects or causes a change, through the direct monitoring and/or control of industrial equipment, assets, processes and events.
- Programmable Logic Controllers: An industrial digital computer which has been ruggedized and adapted for the control of manufacturing processes, such as assembly lines, or robotic devices, or any activity that requires high reliability, ease of programming and process fault diagnosis.
- Supervisory Control and Data Acquisition: A control system architecture comprising of computers, networked data communications and graphical user interfaces for high-level process supervisory management. It also comprising other peripheral devices like programmable logic controllers to interface with process plants or machinery.
- Manufacturing Execution Systems: These are computerized systems used in manufacturing to track and document the transformation of raw materials to finished goods. These systems provide information that helps manufacturing decision makers understand how current conditions on the plant floor can be optimized to improve production output.