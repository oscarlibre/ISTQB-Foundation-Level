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

*Objectives:* Component testing (also known as unit or module testing) focuses on components that are separately testable. Objectives of component testing include:
- Reducing risk 
- Verifying whether the functional and non-functional behaviors of the component are as designed
and specified 
- Building confidence in the component’s quality 
- Finding defects in the component 
- Preventing defects from escaping to higher test levels

---
**NOTE**

Component testing is often done in isolation from the rest of the system, depending on the software development lifecycle model and the system, which may require mock objects, service virtualization, harnesses, stubs, and drivers

---

### Integration Testing 

*Objectives:* Integration testing focuses on interactions between components or systems. Objectives of integration testing include: 
- Reducing risk 
- Verifying whether the functional and non-functional behaviors of the interfaces are as designed
and specified 
- Building confidence in the quality of the interfaces 
- Finding defects (which may be in the interfaces themselves or within the components or systems) - Preventing defects from escaping to higher test levels 

There are two different levels of integration testing described in this syllabus, which may be carried out on test objects of varying size as follows: 

- Component integration testing is performed after component testing, and is
generally automated. In iterative and incremental development, component integration tests are
usually part of the continuous integration process. 

- System integration testing focuses on the interactions and interfaces between systems,
packages, and microservices. System integration testing can also cover interactions with, and
interfaces provided by, external organizations (e.g., web services). In this case, the developing
organization does not control the external interfaces, which can create various challenges for
testing (e.g., ensuring that test-blocking defects in the external organization’s code are resolved,arranging for test environments, etc.). System integration testing may be done after system testing or in parallel with ongoing system test activities (in both sequential development and iterative and incremental development).

