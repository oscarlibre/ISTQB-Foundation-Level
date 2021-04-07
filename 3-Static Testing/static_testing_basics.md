# Static Testing Basics

Static testing relies on the manual examination of work products (i.e., reviews) or tool-driven evaluation of the code or
other work products (i.e., static analysis). Both types of static testing assess the code or other work
product being tested without actually executing the code or work product being tested.

Static analysis is important for safety-critical computer systems , but static analysis has also become 
important and common in other settingssuch as security testing. Static analysis is also often incorporated 
into automated software build and distribution tools, for example in Agile development, continuous delivery,
and continuous deployment.

### Work Products that Can Be Examined by Static Testing 

- Specifications, including business requirements, functional requirements, and security
requirements 
- Epics, user stories, and acceptance criteria 
- Architecture and design specifications 
- Code 
- Testware, including test plans, test cases, test procedures, and automated test scripts 
- User guides 
- Web pages 
- Contracts, project plans, schedules, and budget planning 
- Configuration set up and infrastructure set up 
- Models, such as activity diagrams, which may be used for Model-Based testing 

Reviews can be applied to any work product that the participants know how to read and understand.
Static analysis can be applied efficiently to any work product with a formal structure (typically code or
models) for which an appropriate static analysis tool exists. Static analysis can even be applied with tools
that evaluate work products written in natural language such as requirements (e.g., checking for spelling,
grammar, and readability). 


### Benefits of Static Testing 

When applied early in the software development lifecycle, static testing enables the early detection of 
defects before dynamic testing is performed. Defects found early are often much cheaper to remove than 
defects found later in the lifecycle, especially compared to defects found after the software is deployed
and in active use. Using static testing techniques to find defects and then fixing those defects promptly is 
almost always much cheaper for the organization than using dynamic testing to find defects in the test object 
and then fixing them, especially when considering the additional costs associated with updating other work
products and performing confirmation and regression testing.

Additional benefits of static testing may include:

- Detecting and correcting defects more efficiently, and prior to dynamic test execution 
- Identifying defects which are not easily found by dynamic testing 
- Preventing defects in design or coding by uncovering inconsistencies, ambiguities, contradictions,
omissions, inaccuracies, and redundancies in requirements 
- Increasing development productivity (e.g., due to improved design, more maintainable code) 
- Reducing development cost and time 
- Reducing testing cost and time 
- Reducing total cost of quality over the software’s lifetime, due to fewer failures later in the
lifecycle or after delivery into operation 
- Improving communication between team members in the course of participating in reviews

###  Differences between Static and Dynamic Testing

Static testing and dynamic testing can have the same objectives, such as providing an
assessment of the quality of the work products and identifying defects as early as possible. 
Static and dynamic testing complement each other by finding different types of defects.
One main distinction is that static testing finds defects in work products directly rather than identifying
failures caused by defects when the software is run. A defect can reside in a work product for a very long
time without causing a failure. The path where the defect lies may be rarely exercised or hard to reach, so
it will not be easy to construct and execute a dynamic test that encounters it. Static testing may be able to
find the defect with much less effort. Another distinction is that static testing can be used to improve the 
consistency and internal quality of work products, while dynamic testing typically focuses on externally visible behaviors.

Compared with dynamic testing, typical defects that are easier and cheaper to find and fix through static
testing include: 

- Requirement defects (e.g., inconsistencies, ambiguities, contradictions, omissions, inaccuracies,
and redundancies) 
- Design defects (e.g., inefficient algorithms or database structures, high coupling, low cohesion) 
- Coding defects (e.g., variables with undefined values, variables that are declared but never used,
unreachable code, duplicate code) 
- Deviations from standards (e.g., lack of adherence to coding standards) 
- Incorrect interface specifications (e.g., different units of measurement used by the calling system
than by the called system) 
- Security vulnerabilities (e.g., susceptibility to buffer overflows) 
- Gaps or inaccuracies in test basis traceability or coverage (e.g., missing tests for an acceptance
criterion) 

Moreover, most types of maintainability defects can only be found by static testing (e.g., improper
modularization, poor reusability of components, code that is difficult to analyze and modify without
introducing new defects).
