# Risks and Testing 

### Definition of Risk 

Risk involves the possibility of an event in the future which has negative consequences. The level of risk
is determined by the likelihood of the event and the impact (the harm) from that event. 


### Product and Project Risks 

Product risk involves the possibility that a work product (e.g., a specification, component, system, or test)
may fail to satisfy the legitimate needs of its users and/or stakeholders. When the product risks are
associated with specific quality characteristics of a product (e.g., functional suitability, reliability,
performance efficiency, usability, security, compatibility, maintainability, and portability), product risks are
also called quality risks. Examples of product risks include:

- Software might not perform its intended functions according to the specification 
- Software might not perform its intended functions according to user, customer, and/or stakeholder
needs 
- A system architecture may not adequately support some non-functional requirement(s) 
- A particular computation may be performed incorrectly in some circumstances 
- A loop control structure may be coded incorrectly 
- Response-times may be inadequate for a high-performance transaction processing system 
- User experience (UX) feedback might not meet product expectations

Project risk involves situations that, should they occur, may have a negative effect on a project's ability to
achieve its objectives. Examples of project risks include: 

- Project issues: 
  - Delays may occur in delivery, task completion, or satisfaction of exit criteria or definition of done 
  - Inaccurate estimates, reallocation of funds to higher priority projects, or general costcutting across the organization may result in inadequate funding 
  - Late changes may result in substantial re-work 
  
- Organizational issues: 
  - Skills, training, and staff may not be sufficient 
  - Personnel issues may cause conflict and problems 
  - Users, business staff, or subject matter experts may not be available due to conflicting
business priorities 

- Political issues: 
  - Testers may not communicate their needs and/or the test results adequately 
  - Developers and/or testers may fail to follow up on information found in testing and
reviews (e.g., not improving development and testing practices) 
  - There may be an improper attitude toward, or expectations of, testing (e.g., not
appreciating the value of finding defects during testing) 

- Technical issues: 
  - Requirements may not be defined well enough 
  - The requirements may not be met, given existing constraints 
  - The test environment may not be ready on time 
  - Data conversion, migration planning, and their tool support may be late 
  - Weaknesses in the development process may impact the consistency or quality of project
work products such as design, code, configuration, test data, and test cases 
  - Poor defect management and similar problems may result in accumulated defects and
other technical debt 

- Supplier issues: 
  - A third party may fail to deliver a necessary product or service, or go bankrupt 
  - Contractual issues may cause problems to the project

Project risks may affect both development activities and test activities. In some cases, project managers
are responsible for handling all project risks, but it is not unusual for test managers to have responsibility
for test-related project risks.


### Risk-based Testing and Product Quality

It is used to decide where and when to start testing and **to identify areas that need more attention**. 
Testing is used to reduce the probability of an adverse event occurring, or to reduce the impact of 
an adverse event. **Testing is used as a risk mitigation activity**, to provide information about 
identified risks, as well as providing information on residual (unresolved) risks.

A risk-based approach to testing provides proactive opportunities to reduce the levels of product risk. It
involves product risk analysis, which includes the identification of product risks and the assessment of
each risk’s likelihood and impact. The resulting product risk information is used to guide test planning, the
specification, preparation and execution of test cases, and test monitoring and control. Analyzing product
risks early contributes to the success of a project.

In a risk-based approach, the results of product risk analysis are used to:

- Determine the test techniques to be employed 
- Determine the particular levels and types of testing to be performed (e.g., security testing,
accessibility testing) 
- Determine the extent of testing to be carried out 
- Prioritize testing in an attempt to find the critical defects as early as possible 
- Determine whether any activities in addition to testing could be employed to reduce risk (e.g.,
providing training to inexperienced designers) 

Risk-based testing draws on the collective knowledge and insight of the project stakeholders to carry out
product risk analysis. To ensure that the likelihood of a product failure is minimized, risk management
activities provide a disciplined approach to: 

- Analyze (and re-evaluate on a regular basis) what can go wrong (risks) 
- Determine which risks are important to deal with 
- Implement actions to mitigate those risks 
- Make contingency plans to deal with the risks should they become actual events

In addition, testing may identify new risks, help to determine what risks should be mitigated, and lower
uncertainty about risks. 
