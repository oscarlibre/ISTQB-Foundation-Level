# Test Planning and Estimation 

### Purpose and Content of a Test Plan  

A test plan outlines test activities for development and maintenance projects. Planning is influenced by
the test policy and test strategy of the organization, the development lifecycles and methods being used, 
the scope of testing, objectives, risks, constraints, criticality, testability, and the
availability of resources.

As the project and test planning progress, more information becomes available and more detail can be
included in the test plan. Test planning is a **continuous** activity and is performed throughout the product's
lifecycle. Feedback from test activities should be used to recognize changing risks so that
planning can be adjusted. Planning may be documented in a master test plan and in separate test plans
for test levels, such as system testing and acceptance testing, or for separate test types, such as usability
testing and performance testing. Test planning activities may include the following and some of these
may be documented in a test plan: 

- Determining the scope, objectives, and risks of testing 
- Defining the overall approach of testing 
- Integrating and coordinating the test activities into the software lifecycle activities 
- Making decisions about what to test, the people and other resources required to perform the
various test activities, and how test activities will be carried out 
- Scheduling of test analysis, design, implementation, execution, and evaluation activities, either on
particular dates (e.g., in sequential development) or in the context of each iteration (e.g., in
iterative development) 
- Selecting metrics for test monitoring and control 
- Budgeting for the test activities 
- Determining the level of detail and structure for test documentation (e.g., by providing templates
or example documents)

The content of test plans vary, and can extend beyond the topics identified above. A sample test plan
structure and a sample test plan can be found in ISO standard (ISO/IEC/IEEE 29119-3). 

### Test Strategy and Test Approach

A test strategy provides a generalized description of the test process, usually at the product or
organizational level. Common types of test strategies include: 

- **Analytical**: This type of test strategy is based on an analysis of some factor (e.g., requirement or
risk). Risk-based testing is an example of an analytical approach, where tests are designed and
prioritized based on the level of risk. 
- **Model-Based**: In this type of test strategy, tests are designed based on some model of some
required aspect of the product, such as a function, a business process, an internal structure, or a
non-functional characteristic (e.g., reliability). Examples of such models include business process
models, state models, and reliability growth models. 
- **Methodical**: This type of test strategy relies on making systematic use of some predefined set of
tests or test conditions, such as a taxonomy of common or likely types of failures, a list of 
important quality characteristics, or company-wide look-and-feel standards for mobile apps or
web pages. 
- **Process-compliant** (or standard-compliant): This type of test strategy involves analyzing,
designing, and implementing tests based on external rules and standards, such as those
specified by industry-specific standards, by process documentation, by the rigorous identification
and use of the test basis, or by any process or standard imposed on or by the organization. 
- **Directed** (or consultative): This type of test strategy is driven primarily by the advice, guidance, or
instructions of stakeholders, business domain experts, or technology experts, who may be
outside the test team or outside the organization itself. 
- **Regression-averse**: This type of test strategy is motivated by a desire to avoid regression of
existing capabilities. This test strategy includes reuse of existing testware (especially test cases
and test data), extensive automation of regression tests, and standard test suites. 
- **Reactive**: In this type of test strategy, testing is reactive to the component or system being
tested, and the events occurring during test execution, rather than being pre-planned (as the
preceding strategies are). Tests are designed and implemented, and may immediately be
executed in response to knowledge gained from prior test results. Exploratory testing is a
common technique employed in reactive strategies

An appropriate test strategy is often created by combining several of these types of test strategies. For
example, risk-based testing (an analytical strategy) can be combined with exploratory testing (a reactive
strategy); they complement each other and may achieve more effective testing when used together.
While the test strategy provides a generalized description of the test process, the test approach tailors the
test strategy for a particular project or release. The test approach is the starting point for selecting the test
techniques, test levels, and test types, and for defining the entry criteria and exit criteria (or definition of
ready and definition of done, respectively). The tailoring of the strategy is based on decisions made in
relation to the complexity and goals of the project, the type of product being developed, and product risk
analysis. The selected approach depends on the context and may consider factors such as risks, safety,
available resources and skills, technology, the nature of the system (e.g., custom-built versus COTS), test
objectives, and regulations. 


### Entry Criteria and Exit Criteria (Definition of Ready and Definition of Done)

In order to exercise effective control over the quality of the software, and of the testing, it is advisable to
have criteria which define when a given test activity should start and when the activity is complete. Entry
criteria (more typically called definition of ready in Agile development) define the preconditions for
undertaking a given test activity. If entry criteria are not met, it is likely that the activity will prove more
difficult, more time-consuming, more costly, and more risky. Exit criteria (more typically called definition of
done in Agile development) define what conditions must be achieved in order to declare a test level or a
set of tests completed. Entry and exit criteria should be defined for each test level and test type, and will
differ based on the test objectives. 

Typical entry criteria include: 

- Availability of testable requirements, user stories, and/or models (e.g., when following a modelbased testing strategy) 
- Availability of test items that have met the exit criteria for any prior test levels
- Availability of test environment 
- Availability of necessary test tools 
- Availability of test data and other necessary resources

Typical exit criteria include: 

- Planned tests have been executed 
- A defined level of coverage (e.g., of requirements, user stories, acceptance criteria, risks, code)
has been achieved 
- The number of unresolved defects is within an agreed limit 
- The number of estimated remaining defects is sufficiently low 
- The evaluated levels of reliability, performance efficiency, usability, security, and other relevant
quality characteristics are sufficient

Even without exit criteria being satisfied, it is also common for test activities to be curtailed due to the budget being expended, the scheduled time being completed, and/or pressure to bring the product to
market. It can be acceptable to end testing under such circumstances, if the project stakeholders and
business owners have reviewed and accepted the risk to go live without further testing. 


### Factors Influencing the Test Effort

Test effort estimation involves predicting the amount of test-related work that will be needed in order to
meet the objectives of the testing for a particular project, release, or iteration. Factors influencing the test effort may include characteristics of the product, characteristics of the development process,
characteristics of the people, and the test results, as shown below. 

Product characteristics 

- The risks associated with the product 
- The quality of the test basis 
- The size of the product 
- The complexity of the product domain 
- The requirements for quality characteristics (e.g., security, reliability) 
- The required level of detail for test documentation 
- Requirements for legal and regulatory compliance

Development process characteristics 

- The stability and maturity of the organization 
- The development model in use 
- The test approach 
- The tools used 
- The test process 
- Time pressure

People characteristics 

- The skills and experience of the people involved, especially with similar projects and products
(e.g., domain knowledge) 
- Team cohesion and leadership

Test results 

- The number and severity of defects found 
- The amount of rework required


### Test Estimation Techniques

There are a number of estimation techniques used to determine the effort required for adequate testing.
Two of the most commonly used techniques are: 

- *The metrics-based technique*: estimating the test effort based on metrics of former similar
projects, or based on typical values 
- *The expert-based technique*: estimating the test effort based on the experience of the owners of
the testing tasks or by experts

For example, in Agile development, burndown charts are examples of the metrics-based approach as
effort remaining is being captured and reported, and is then used to feed into the team’s velocity to
determine the amount of work the team can do in the next iteration; whereas planning poker is an
example of the expert-based approach, as team members are estimating the effort to deliver a feature
based on their experience.

Within sequential projects, defect removal models are examples of the metrics-based approach, where
volumes of defects and time to remove them are captured and reported, which then provides a basis for
estimating future projects of a similar nature; whereas the Wideband Delphi estimation technique is an
example of the expert-based approach in which a group of experts provides estimates based on their
experience.



