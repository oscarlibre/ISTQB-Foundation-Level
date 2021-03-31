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
programming languages) or the particular user base.


### White-box Testing

White-box testing derives tests based on the system’s internal structure or implementation, it may include code, architecture, work flows, and/or data flows within the system.

The thoroughness of white-box testing can be measured through structural coverage. At the component testing level, code coverage is based on the percentage of component code that has been tested, and may be measured in terms of different aspects of code (coverage items) such as the percentage of executable statements tested in the component, or the percentage of decision outcomestested. These types of coverage are collectively called code coverage. 

At the component integration testing level, white-box testing may be based on the architecture of the system, such as interfaces between components, and structural coverage may be measured in terms of the percentage of interfaces
exercised by tests. White-box test design and execution may involve special skills or knowledge, such as the way the code is built, how data is stored (e.g., to evaluate possible database queries), and how to use coverage tools and
to correctly interpret their results. 


### Change-related Testing

When changes are made to a system, either to correct a defect or because of new or changing
functionality, testing should be done to confirm that the changes have corrected the defect or
implemented the functionality correctly, and have not caused any unforeseen adverse consequences. 

- *Confirmation testing:* The purpose of a confirmation test is to confirm whether the original defect has been
successfully fixed. The software may also be tested with new tests to cover changes needed to fix the defect.

- *Regression testing:* It is possible that a change made in one part of the code, whether a fix or
another type of change, may accidentally affect the behavior of other parts of the code, whether
within the same component, in other components of the same system, or even in other systems.
Changes may include changes to the environment, such as a new version of an operating system
or database management system. Such unintended side-effects are called regressions.
Regression testing involves running tests to detect such unintended side-effects.

Confirmation testing and regression testing are performed at all test levels.
Especially in iterative and incremental development lifecycles (e.g., Agile), new features, changes to
existing features, and code refactoring result in frequent changes to the code, which also requires
change-related testing. Due to the evolving nature of the system, confirmation and regression testing are
very important. This is particularly relevant for Internet of Things systems where individual objects (e.g.,
devices) are frequently updated or replaced.
Regression test suites are run many times and generally evolve slowly, so regression testing is a strong
candidate for automation. Automation of these tests should start early in the project.
