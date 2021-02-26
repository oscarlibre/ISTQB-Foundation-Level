# Test Process

- There is no one universal software test process
- There are common sets of test activities that help to achieve its established objectives (These sets of test activities are a test process.)
- The proper, specific software test process in any given situation depends on many factors:
	- Which test activities are involved in this test process
	- How these activities are implemented
	- when these activities occur 

### Test Process in Context 

- Software development lifecycle model and project methodologies being used 
- Test levels and test types being considered 
- Product and project risks 
- Business domain 
- Operational constraints, including but not limited to: 
	o Budgets and resources o Timescales 
	o Complexity 
	o Contractual and regulatory requirements 
- Organizational policies and practices 
- Required internal and external standards

---
**NOTE**

It is very useful if the test basis (for any level or type of testing that is being considered) has measurable
coverage criteria defined. The coverage criteria can act effectively as key performance indicators (KPIs)
to drive the activities that demonstrate achievement of software test objectives.

---

![Test processes ISO/IEC/IEEE 29119-2](https://www.iso.org/standard/56736.html)


### Test Activities and Tasks 

A test process consists of the following main groups of activities: 

**Test planning**:  It involves activities that define the objectives of testing and the approach for meeting test
objectives within constraints imposed by the context  Test plans may be revisited based on feedback from monitoring 
and control activities

**Test monitoring and control**: Test monitoring involves the on-going comparison of actual progress against planned progress using any
test monitoring metrics defined in the test plan. Test control involves taking actions necessary to meet the
objectives of the test plan (which may be updated over time). Test monitoring and control are supported
by the evaluation of exit criteria, which are referred to as the definition of done in some software
development lifecycle models. For example, the evaluation of exit criteria for test
execution as part of a given test level may include:

- Checking test results and logs against specified coverage criteria 
- Assessing the level of component or system quality based on test results and logs 
- Determining if more tests are needed (e.g., if tests originally intended to achieve a certain level of
product risk coverage failed to do so, requiring additional tests to be written and executed)

Test progress against the plan is communicated to stakeholders in test progress reports, including
deviations from the plan and information to support any decision to stop testing.

**Test analysis**: Test analysis determines “what to test” in terms of measurable coverage.
criteria. Test analysis includes the following major activities: 

- Analyzing the test basis appropriate to the test level being considered, for example:
	
	- Requirement specifications, such as business requirements, functional requirements,
	system requirements, user stories, epics, use cases, or similar work products that specify	
	desired functional and non-functional component or system behavior

	- Design and implementation information, such as system or software architecture
	diagrams or documents, design specifications, call flow graphs, modelling diagrams, 
	interface specifications, or similar work products that specify component or system structure
	
	- The implementation of the component or system itself, including code, database metadata and queries, 
	and interfaces 
	
	- Risk analysis reports, which may consider functional, non-functional, and structural
	aspects of the component or system 
	
- Evaluating the test basis and test items to identify defects of various types, such as:
	- Ambiguities 
	- Omissions 
	- Inconsistencies 
	- Inaccuracies
	- Contradictions
	- Superfluous statements
	- Identifying features and sets of features to be tested 
	- Defining and prioritizing test conditions for each feature based on analysis of the test basis, and
	considering functional, non-functional, and structural characteristics, other business and technical
	factors, and levels of risks 
	- Capturing bi-directional traceability between each element of the test basis and the associated
	test conditions

- Other considerations:
	- The application of black-box, white-box, and experience-based test techniques can be useful in the
	process of test analysis to reduce the likelihood of omitting important test conditions and
	to define more precise and accurate test conditions. 

	- The identification of defects during test analysis is an important potential benefit, especially where no
	other review process is being used and/or the test process is closely connected with the review process.

	- test analysis activities not only verify whether the requirements are consistent, properly expressed,
	and complete, but also validate whether the requirements properly capture customer, user, and other
	stakeholder needs

	- Techniques such as behavior driven development (BDD) and acceptance test driven development (ATDD), 
	which involve generating test conditions and test cases from user stories and acceptance criteria prior to coding. 
	These techniques also verify, validate, and detect defects in the user stories and acceptance criteria
