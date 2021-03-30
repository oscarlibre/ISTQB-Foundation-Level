# Test Types 

A test type is a group of test activities aimed at testing specific characteristics of a software system, or a
part of a system, based on specific test objectives. Such objectives may include: 

- Evaluating functional quality characteristics, such as completeness, correctness, and
appropriateness 
- Evaluating non-functional quality characteristics, such as reliability, performance efficiency,
security, compatibility, and usability 
- Evaluating whether the structure or architecture of the component or system is correct, complete,
and as specified 
- Evaluating the effects of changes, such as confirming that defects have been fixed (confirmation
testing) and looking for unintended changes in behavior resulting from software or environment
changes (regression testing)


![imagen](https://user-images.githubusercontent.com/2337039/113053717-38c81980-916e-11eb-8543-fc2eafa6cc47.png)
![ISO/IEC 25010 for a classification of software product quality characteristics]("https://iso25000.com/index.php/en/iso-25000-standards/iso-25010")

### Functional Testing

It involves tests that evaluate functions that the system should perform. The functions are “what” the system should do.
Functional requirements may be described in work products such as:
  
  - Business requirements
  - Specifications 
  - Epics 
  - User stories 
  - Use cases 
  - Functional specifications
  - Also they may be undocumented.

Functional tests should be performed at all test levels though the focus is different at each level. Functional testing considers 
the behavior of the software, so black-box techniques may be used to derive test conditions and test cases for the functionality 
of the component or system.

The thoroughness of functional testing can be measured through functional coverage. Functional
coverage is the extent to which some functionality has been exercised by tests, and is expressed as a
percentage of the type(s) of element being covered. For example, using traceability between tests and
functional requirements, the percentage of these requirements which are addressed by testing can be
calculated, potentially identifying coverage gaps. 

Functional test design and execution may involve special skills or knowledge, such as knowledge of the
particular business problem the software solves.

### Non-functional Testing

Non-functional testing of a system evaluates characteristics of systems and software such as usability,
performance efficiency or security. Non-functional testing is the testing of “how well” the system behaves.

---
**NOTE**

Contrary to common misperceptions, non-functional testing can and often should be performed at all test
levels, and done as early as possible. The late discovery of non-functional defects can be extremely
dangerous to the success of a project.

---

Black-box techniques may be used to derive test conditions and test cases for nonfunctional testing. 
For example, boundary value analysis can be used to define the stress conditions for
performance tests.

The thoroughness of non-functional testing can be measured through non-functional coverage. 
Nonfunctional coverage is the extent to which some type of non-functional element has been exercised by
tests, and is expressed as a percentage of the type(s) of element being covered. For example, using
traceability between tests and supported devices for a mobile application, the percentage of devices
which are addressed by compatibility testing can be calculated, potentially identifying coverage gaps.
Non-functional test design and execution may involve special skills or knowledge, such as knowledge of
the inherent weaknesses of a design or technology (e.g., security vulnerabilities associated with particular
programming languages) or the particular user base 

