# Test Monitoring and Control

The purpose of test monitoring is to gather information and provide feedback and visibility about test
activities. Information to be monitored may be collected manually or automatically and should be used to
assess test progress and to measure whether the test exit criteria, or the testing tasks associated with an
Agile project's definition of done, are satisfied, such as meeting the targets for coverage of product risks,
requirements, or acceptance criteria.

Test control describes any guiding or corrective actions taken as a result of information and metrics
gathered and (possibly) reported. Actions may cover any test activity and may affect any other software
lifecycle activity. 

Examples of test control actions include:

- Re-prioritizing tests when an identified risk occurs 
- Changing the test schedule due to availability or unavailability of a test environment or other
resources 
- Re-evaluating whether a test item meets an entry or exit criterion due to rework 


### Metrics Used in Testing 

Metrics can be collected during and at the end of test activities in order to assess: 

- Progress against the planned schedule and budget 
- Current quality of the test object 
- Adequacy of the test approach 
- Effectiveness of the test activities with respect to the objectives

Common test metrics include: 

- Percentage of planned work done in test case preparation (or percentage of planned test cases
implemented) 
- Percentage of planned work done in test environment preparation 
- Test case execution (e.g., number of test cases run/not run, test cases passed/failed, and/or test
conditions passed/failed) 
- Defect information (e.g., defect density, defects found and fixed, failure rate, and confirmation test
results) 
- Test coverage of requirements, user stories, acceptance criteria, risks, or code 
- Task completion, resource allocation and usage, and effort 
- Cost of testing, including the cost compared to the benefit of finding the next defect or the cost
compared to the benefit of running the next test

### Purposes, Contents, and Audiences for Test Reports

The purpose of test reporting is to summarize and communicate test activity information, both during and
at the end of a test activity (e.g., a test level). The test report prepared during a test activity may be
referred to as a test progress report, while a test report prepared at the end of a test activity may be
referred to as a test summary report.

During test monitoring and control, the test manager regularly issues test progress reports for
stakeholders. In addition to content common to test progress reports and test summary reports, typical
test progress reports may also include:

- The status of the test activities and progress against the test plan 
- Factors impeding progress 
- Testing planned for the next reporting period 
- The quality of the test object

When exit criteria are reached, the test manager issues the test summary report. This report provides a
summary of the testing performed, based on the latest test progress report and any other relevant
information.

Typical test summary reports may include: 

- Summary of testing performed 
- Information on what occurred during a test period 
- Deviations from plan, including deviations in schedule, duration, or effort of test activities 
- Status of testing and product quality with respect to the exit criteria or definition of done 
- Factors that have blocked or continue to block progress 
- Metrics of defects, test cases, test coverage, activity progress, and resource consumption. 
- Residual risks
- Reusable test work products produced 

The contents of a test report will vary depending on the project, the organizational requirements, and the
software development lifecycle. For example, a complex project with many stakeholders or a regulated
project may require more detailed and rigorous reporting than a quick software update. As another
example, in Agile development, test progress reporting may be incorporated into task boards, defect
summaries, and burndown charts, which may be discussed during a daily stand-up meeting.

In addition to tailoring test reports based on the context of the project, test reports should be tailored
based on the report’s audience. The type and amount of information that should be included for a
technical audience or a test team may be different from what would be included in an executive summary
report. In the first case, detailed information on defect types and trends may be important. In the latter
case, a high-level report (e.g., a status summary of defects by priority, budget, schedule, and test
conditions passed/failed/not tested) may be more appropriate.

ISO standard (ISO/IEC/IEEE 29119-3) refers to two types of test reports, test progress reports and test
completion reports (called test summary reports), and contains structures and examples
for each type. 
