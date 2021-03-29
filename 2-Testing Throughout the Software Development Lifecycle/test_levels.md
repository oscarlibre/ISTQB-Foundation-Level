# Test Levels 

Test levels are groups of test activities that are organized and managed together. Each test level is an
instance of the test process, consisting of the activities, performed in relation to software at a given level of development, 
from individual units or components to complete systems or, where applicable, systems of systems.
Test levels are related to other activities within the software development lifecycle. 

Most common test levels:

- Component testing 
- Integration testing 
- System testing 
- Acceptance testing

Test levels are characterized by the following attributes: 

- Specific objectives 
- Test basis
- Referenced to derive test cases 
- Test object (i.e., what is being tested) 
- Typical defects and failures 
- Specific approaches and responsibilities 

---
**NOTE**

For every test level, a suitable test environment is required. In acceptance testing, for example, a
production-like test environment is ideal, while in component testing the developers typically use their
own development environment. 

---

### Component Testing 

- Component testing (also known as unit or module testing) focuses on components that are separately testable.
- In some cases, automated component regression tests play a key role in building confidence that  changes have not broken existing components (e.g Agile). 
- Component testing is often done in isolation from the rest of the system, depending on the software
development lifecycle model and the system, which may require mock objects, service virtualization,
harnesses, stubs, and drivers. 
- Component testing may cover functionality (e.g., correctness of
calculations), non-functional characteristics (e.g., searching for memory leaks), and structural properties
(e.g., decision testing).
- Defects are typically fixed as soon as they are found, often with no formal defect management. However,
when developers do report defects, this provides important information for root cause analysis and
process improvement. 

### Integration Testing 

- Integration testing focuses on interactions between components or systems.
- In some cases automated integration regression tests provide confidence that
changes have not broken existing interfaces, components, or systems. 
- There are two different levels of integration testing which may be carried out on test objects of varying size as follows: 

  - *Component integration testing:* It is performed after component testing (generally automated). In iterative and incremental development, component integration tests are usually part of the continuous integration process. 

  - *System integration testing*: It focuses on the interactions and interfaces between systems,
packages, and microservices. System integration testing can also cover interactions with, and
interfaces provided by, external organizations (e.g., web services). In this case, the developing
organization does not control the external interfaces, which can create various challenges for
testing (e.g., ensuring that test-blocking defects in the external organization’s code are resolved,arranging for test environments, etc.). System integration testing may be done after system testing or in parallel with ongoing system test activities (in both sequential development and iterative and incremental development).


### System Testing 

System testing focuses on the behavior and capabilities of a whole system or product, often considering the end-to-end tasks the system can perform and the non-functional behaviors it exhibits while performing those tasks.

---
**NOTE**

In some cases automated system regression tests provide confidence that changes
have not broken existing features or end-to-end capabilities. System testing often produces information that is used by stakeholders to make release decisions. System testing may also satisfy legal or regulatory requirements or standards. The test environment should ideally correspond to the final target or production environment.

---

### Acceptance Testing 

It typically focuses on the behavior and capabilities of a whole system or product. Acceptance testing may produce information to assess the system’s readiness for deployment and use by the customer (end-user). Defects may be found during acceptance testing, 
but finding defects is often not an objective, and finding a significant number of defects 
during acceptance testing may in some cases be considered a major project risk. 
Acceptance testing may also satisfy legal or regulatory requirements or standards.

Common forms of acceptance testing include the following: 

- *User acceptance testing (UAT):* The main objective is building confidence that the users
 can use the system to meet their needs, fulfill requirements, and perform business processes
 with minimum difficulty, cost, and risk. 

- *Operational acceptance testing (OAT):* The acceptance testing of the system by operations
 or systems administration staff is usually performed in a (simulated) production environment.
 The tests focus on operational aspects, and may include: 
	- Testing of backup and restore 
	- Installing, uninstalling and upgrading 
	- Disaster recovery 
	- User management 
	- Maintenance tasks 
	- Data load and migration tasks 
	- Checks for security vulnerabilities 
	- Performance testing 
	
  The main objective of operational acceptance testing is building confidence that the operators or system
	administrators can keep the system working properly for the users in the operational environment, even
	under exceptional or difficult conditions. 

- *Contractual and regulatory acceptance testing:* Contractual acceptance testing is performed
 against a contract’s acceptance criteria for producing custom-developed software. 
 Acceptance criteria should be defined when the parties agree to the contract. 
 Contractual acceptance testing is often performed by users or by independent testers.
 Regulatory acceptance testing is performed against any regulations that must be adhered to,
 such as government, legal, or safety regulations. Regulatory acceptance testing is often 
 performed by users or by independent testers, sometimes with the results being witnessed
 or audited by regulatory agencies. The main objective of contractual and regulatory 
 acceptance testing is building confidence that contractual or regulatory compliance has
 been achieved. 

- *Alpha and beta testing:* One objective of alpha and beta testing is building confidence among 
 potential or existing customers, and/or operators that they can use the system under normal, 
 everyday conditions, and in the operational environment(s) to achieve their objectives with 
 minimum difficulty, cost, and risk. Another objective may be the detection of defects related to 
 the conditions and environment(s) in which the system will be used, especially when those 
 conditions and environment(s) are difficult to replicate by the development team. Alpha testing is 
 performed at the developing organization’s site by potential or existing customers, and/or operators or
 an independent test team, on the other hand Beta testing is performed at their own locations.



### Test Levels comparison table

|                         | Objectives                                                                                                                                                                                                                                                                                                                                                                   | Test basis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Test objects                                                                                                                                                                                                                                                                                                                                 | Defects & failures                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Approaches & responsibilities                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|-------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Component testing**   | - Reducing risks<br>- Verifying functional & non-functional behaviors of components are as designed and specified<br>- Building confidence in component's quality<br>- Finding defects in components<br>- Preventing defects from scaping to higher layers                                                                                                                   | - Detailed design<br>- Code<br>- Data Model<br>- Component specifications                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | - Components, units or modules<br>- Code and data structures<br>- Classes<br>- Database modules                                                                                                                                                                                                                                              | - Incorrect functionality (e.g not as described in design specifications)<br>- Data flow problems<br>- Incorrect code and logic                                                                                                                                                                                                                                                                                                                                                                                                                 | - Usually performed by the developer who wrote the code<br>- Developers often write and execute tests after having written the code for a component<br>- In Agile development especially, writing automated component test cases may precede writing application codebv (e.g TDD)                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Integration testing** | - Reducing risk <br>- Verifying functional and non-functional behaviors of the interfaces are as designed<br>and specified <br>- Building confidence in the quality of the interfaces <br>- Finding defects (which may be in the interfaces themselves or within the components or systems) <br>- Preventing defects from escaping to higher test levels                     | - Software and system design <br>- Sequence diagrams <br>- Interface and communication protocol specifications <br>- Use cases <br>- Architecture at component or system level<br>- Workflows <br>- External interface definitions                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | - Subsystems<br>- Databases <br>- Infrastructure <br>- Interfaces <br>- APIs <br>- Microservices                                                                                                                                                                                                                                             | - Incorrect data, missing data, or incorrect data encoding <br>- Incorrect sequencing or timing of interface calls <br>- Interface mismatch <br>- Failures in communication between components or systems<br>- Unhandled or improperly handled communication failures between components or systems<br>-Incorrect assumptions about the meaning, units, or boundaries of the data being passed between<br>components or systems<br>- Inconsistent message structures between systems<br>- Failure to comply with mandatory security regulations | - Component integration testing is often the responsibility of developers<br>- System integration testing is generally the responsibility of testers<br>- Ideally, testers should understand the system architecture, and should have influenced integration planning.<br>- Integration should normally be incremental (i.e., a small number of additional components or systems at a time) <br>- A risk analysis of the most complex interfaces can help to focus the integration testing. <br>- The greater the scope of integration, the more difficult it becomes to isolate defects to a specific<br>component or system,  which may lead to increased risk and additional time for troubleshooting. |
| **System testing**      | - Reducing risk <br>- Verifying whether the functional and non-functional behaviors of the system are as designed and<br>specified <br>- Validating that the system is complete and will work as expected <br>- Building confidence in the quality of the system as a whole <br>- Finding defects <br>- Preventing defects from escaping to higher test levels or production | - System and software requirement specifications (functional and non-functional) <br>- Risk analysis reports <br>- Use cases <br>- Epics and user stories <br>- Models of system behavior <br>- State diagrams <br>- System and user manuals                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | - Applications <br>- Hardware/software systems <br>- Operating systems <br>- System under test (SUT) <br>- System configuration and configuration data                                                                                                                                                                                       | - Incorrect calculations <br>- Incorrect or unexpected system functional or non-functional behavior <br>- Incorrect control and/or data flows within the system <br>- Failure to properly and completely carry out end-to-end functional tasks <br>- Failure of the system to work properly in the system environment(s) <br>- Failure of the system to work as described in system and user manuals                                                                                                                                            | - It should focus on the overall, end-to-end behavior of the system as a whole<br>- It is typically carried out by independent testers who rely heavily on specifications<br>- Defects in specifications can lead to a lack of understanding of, or disagreements about, expected system behavior. Such situations can cause false positives and false negatives, which waste time and reduce defect detection effectiveness,<br>respectively. <br>- Early involvement of testers in user story refinement or static testing activities helps to reduce the incidence of such situations.                                                                                                                 |
| **Acceptance testing**  | - Establishing confidence in the quality of the system as a whole <br>- Validating that the system is complete and will work as expected <br>- Verifying that functional and non-functional behaviors of the system are as specified                                                                                                                                         | - Business processes <br>- User or business requirements <br>- Regulations, legal contracts and standards <br>- Use cases and/or user stories <br>- System requirements <br>- System or user documentation <br>- Installation procedures <br>- Risk analysis reports<br><br>In addition, as a test basis for deriving test cases for operational acceptance testing, one <br>or more of the following work products can be used: <br><br>- Backup and restore procedures <br>- Disaster recovery procedures <br>- Non-functional requirements <br>- Operations documentation <br>- Deployment and installation instructions <br>- Performance targets <br>- Database packages <br>- Security standards or regulations | - System under test <br>- System configuration and configuration data <br>- Business processes for a fully integrated system <br>- Recovery systems and hot sites (for business continuity and disaster recovery testing) <br>- Operational and maintenance processes <br>- Forms <br>- Reports <br>- Existing and converted production data | - System workflows do not meet business or user requirements <br>- Business rules are not implemented correctly <br>- System does not satisfy contractual or regulatory requirements <br>- Non-functional failures such as security vulnerabilities, inadequate performance efficiency under<br>high loads, or improper operation on a supported platform                                                                                                                                                                                       | - Acceptance testing is often the responsibility of the customers, business users, product owners, or<br>operators of a system, and other stakeholders may be involved as well.<br>- Acceptance testing of a COTS (commercial off-the-shelf) software product may occur when it is installed or integrated <br><br>- Acceptance testing of a new functional enhancement may occur before system testing                                                                                                                                                                                                                                                                                                   |


