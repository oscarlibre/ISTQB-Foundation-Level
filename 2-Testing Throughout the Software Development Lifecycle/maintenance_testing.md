# Maintenance Testing 

Software and systems need to be maintained, so the changes of various sorts are almost inevitable in delivered software and systems
either to fix defects discovered, to add new functionality, or to delete or alter already-delivered functionality. 

Maintenance is also needed to preserve or improve non-functional quality characteristics of the component or system
over its lifetime, especially performance efficiency, compatibility, reliability, security, and portability.

When any changes are made as part of maintenance, maintenance testing should be performed, both to
evaluate the success with which the changes were made and to check for possible side-effects (e.g.,
regressions) in parts of the system that remain unchanged (which is usually most of the system).
Maintenance can involve planned releases and unplanned releases (hot fixes).

A maintenance release may require maintenance testing at multiple test levels, using various test types,
based on its scope. The scope of maintenance testing depends on: 

- The degree of risk of the change, for example, the degree to which the changed area of software
communicates with other components or systems 
- The size of the existing system 
- The size of the change 


### Triggers for Maintenance 

We can classify the triggers for maintenance as follows: 

- *Modification*, such as planned enhancements, corrective and emergency
changes, changes of the operational environment (such as planned operating system or
database upgrades), upgrades of COTS software, and patches for defects and vulnerabilities 

- *Migration*, such as from one platform to another, which can require operational tests of the new
environment as well as of the changed software, or tests of data conversion when data from
another application will be migrated into the system being maintained.

  - Retirement, such as when an application reaches the end of its life. When an application
or system is retired, this can require testing of data migration or archiving if long dataretention periods are required. 
  - Testing restore/retrieve procedures after archiving for long retention periods may also be
needed. 
  - Regression testing may be needed to ensure that any functionality that remains in service
still works.

For Internet of Things systems, maintenance testing may be triggered by the introduction of completely
new or modified things, such as hardware devices and software services, into the overall system. The
maintenance testing for such systems places particular emphasis on integration testing at different levels
(e.g., network level, application level) and on security aspects, in particular those relating to personal
data. 


###  Impact Analysis for Maintenance 

- Impact analysis evaluates the changes that were made for a maintenance release to identify the intended
consequences as well as expected and possible side effects of a change.
-  Identify the areas in the system that will be affected by the change. 
-  It helps to identify the impact of a change on existing tests. 
-  Impact analysis may be done before a change is made, to help decide if the change should be made, based on the potential consequences in other areas of the system
  
---
**NOTE**

The side effects and affected areas in the system need to be tested for regressions, possibly after updating any existing tests affected by the change. 

---

Impact analysis can be difficult if: 

- Specifications (e.g., business requirements, user stories, architecture) are out of date or missing 
- Test cases are not documented or are out of date 
- Bi-directional traceability between tests and the test basis has not been maintained 
- Tool support is weak or non-existent 
- The people involved do not have domain and/or system knowledge 
- Insufficient attention has been paid to the software's maintainability during development
