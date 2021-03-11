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
	
**Test design**:  The test conditions are elaborated into high-level test cases, sets of high-level test
cases, and other testware. So, test design answers the question "how to test?". Test design includes the following major activities: 

- Dsigning and prioritizing test cases and sets of test cases
- Identifying necessary test data to support test conditions and test cases
- Designing the test environment and identifying any required infrastructure and tools
- Capturing bi-directional traceability between the test basis, test conditions, and test cases 

The elaboration of test conditions into test cases and sets of test cases during test design often involves
using test techniques. As with test analysis, test design may also result in the identification of similar types of defects in the test
basis. Also, as with test analysis, the identification of defects during test design is an important potential
benefit. 

**Test implementation**:  The testware necessary for test execution is created and/or completed,
including sequencing the test cases into test procedures.  Test implementation answers the question 
"do we now have everything in place to run the tests?".Test implementation includes the following major activities: 

- Developing and prioritizing test procedures, and, potentially, creating automated test scripts 
- Creating test suites from the test procedures and (if any) automated test scripts 
- Arranging the test suites within a test execution schedule in a way that results in efficient test
execution  
- Building the test environment (including, potentially, test harnesses, service virtualization,
simulators, and other infrastructure items) and verifying that everything needed has been set up
correctly 
- Preparing test data and ensuring it is properly loaded in the test environment 
- Verifying and updating bi-directional traceability between the test basis, test conditions, test
cases, test procedures, and test suites

Test design and test implementation tasks are often combined.In exploratory testing and other 
types of experience-based testing, test design and implementation may occur, and may be documented, 
as part of test execution. Exploratory testing may be based on test charters (produced as part of 
test analysis), and exploratory tests are executed immediately as they are designed and implemented.

**Test execution**: Test suites are run in accordance with the test execution schedule.Test execution includes the following major activities:

- Recording the IDs and versions of the test item(s) or test object, test tool(s), and testware
- Executing tests either manually or by using test execution tools 
- Comparing actual results with expected results 
- Analyzing anomalies to establish their likely causes 
- Reporting defects based on the failures observed 
- Logging the outcome of test execution (e.g., pass, fail, blocked)
- Repeating test activities either as a result of action taken for an anomaly, or as part of the
planned testing (e.g., execution of a corrected test, confirmation testing, and/or regression
testing)
- Verifying and updating bi-directional traceability between the test basis, test conditions, test
cases, test procedures, and test results. 

**Test completion**: Test completion activities collect data from completed test activities to consolidate experience, testware,
and any other relevant information. Test completion activities occur at project milestones such as when a
software system is released, a test project is completed (or cancelled), an Agile project iteration is
finished, a test level is completed, or a maintenance release has been completed. Test completion includes the following major activities: 

- Checking whether all defect reports are closed, entering change requests or product backlog
items for any defects that remain unresolved at the end of test execution 
- Creating a test summary report to be communicated to stakeholders 
- Finalizing and archiving the test environment, the test data, the test infrastructure, and other
testware for later reuse 
- Handing over the testware to the maintenance teams, other project teams, and/or other
stakeholders who could benefit from its use 
- Analyzing lessons learned from the completed test activities to determine changes needed for
future iterations, releases, and projects 
- Using the information gathered to improve test process maturity

###  Traceability between the Test Basis and Test Work Products

It is important to establish and maintain traceability throughout the test process between each element of
the test basis and the various test work products associated with that element. In addition to the evaluation
of test coverage, good traceability supports:

- Analyzing the impact of changes 
- Making testing auditable 
- Meeting IT governance criteria 
- Improving the understandability of test progress reports and test summary reports to include the
status of elements of the test basis (e.g., requirements that passed their tests, requirements that
failed their tests, and requirements that have pending tests) 
- Relating the technical aspects of testing to stakeholders in terms that they can understand 
- Providing information to assess product quality, process capability, and project progress against
business goals

---
**NOTE**

Some test management tools provide test work product models that match part or all of the test work
products. Some organizations build their own management systems to organize
the work products and provide the information traceability they require. 

---

