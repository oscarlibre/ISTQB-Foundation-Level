# Review Process

Reviews vary from informal to formal. Informal reviews are characterized by not following a defined
process and not having formal documented output. Formal reviews are characterized by team
participation, documented results of the review, and documented procedures for conducting the review. 

### Work Product Review Process

The review process comprises the following main activities:

| Activity                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *Planning*                         | - Defining the scope, which includes the purpose of the review, what documents or parts of<br>documents to review, and the quality characteristics to be evaluated <br>- Estimating effort and timeframe <br>- Identifying review characteristics such as the review type with roles, activities, and checklists <br>- Selecting the people to participate in the review and allocating roles <br>- Defining the entry and exit criteria for more formal review types (e.g., inspections) <br>- Checking that entry criteria are met (for more formal review types)                                                                                 |
| *Initiate review*                  | - Distributing the work product (physically or by electronic means) and other material, such as<br>issue log forms, checklists, and related work products <br>- Explaining the scope, objectives, process, roles, and work products to the participants <br>- Answering any questions that participants may have about the review                                                                                                                                                                                                                                                                                                                   |
| *Individual review*                | - Reviewing all or part of the work product <br>- Noting potential defects, recommendations, and questions                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| *Issue communication and analysis* | - Communicating identified potential defects (e.g., in a review meeting) <br>- Analyzing potential defects, assigning ownership and status to them <br>- Evaluating and documenting quality characteristics <br>- Evaluating the review findings against the exit criteria to make a review decision (reject; major<br>changes needed; accept, possibly with minor changes)                                                                                                                                                                                                                                                                         |
| *Fixing and Reporting*             | - Creating defect reports for those findings that require changes to a work product <br>- Fixing defects found (typically done by the author) in the work product reviewed <br>- Communicating defects to the appropriate person or team (when found in a work product related<br>to the work product reviewed) <br>- Recording updated status of defects (in formal reviews), potentially including the agreement of<br>the comment originator <br>- Gathering metrics (for more formal review types) <br>- Checking that exit criteria are met (for more formal review types) <br>- Accepting the work product when the exit criteria are reached |


### Roles and responsibilities in a formal review 

A typical formal review will include the roles below: 

| Role                      | Responsibilities                                                                                                                                                                                                                                                                                                                                                                        |
|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *Author*                  | - Creates the work product under review<br>- Fixes defects in the work product under review (if necessary)                                                                                                                                                                                                                                                                              |
| *Management*              | - Review planning <br>- Decides on the execution of reviews <br>- Assigns staff, budget, and time <br>- Monitors ongoing cost-effectiveness <br>- Executes control decisions in the event of inadequate outcomes                                                                                                                                                                        |
| *Facilitator (Moderator)* | - Ensures effective running of review meetings (when held) <br>- Mediates, if necessary, between the various points of view <br>- Is often the person upon whom the success of the review depends                                                                                                                                                                                       |
| *Review Leader*           | - Takes overall responsibility for the review <br>- Decides who will be involved and organizes when and where it will take place                                                                                                                                                                                                                                                        |
| *Reviewers*               | - May be subject matter experts, persons working on the project, stakeholders with an interest in the work product, and/or individuals with specific technical or business backgrounds <br>- Identify potential defects in the work product under review <br>- May represent different perspectives (e.g., tester, developer, user, operator, business analyst, usability expert, etc.) |
| *Scribe (Recorder)*       | - Collates potential defects found during the individual review activity <br>- Records new potential defects, open points, and decisions from the review meeting (when held)                                                                                                                                                                                                            |

---
**NOTE**

One person may play more than one role, and the actions associated with each role
may also vary based on review type. In addition, with the advent of tools to support the review process,
especially the logging of defects, open points, and decisions, there is often no need for a scribe. 

---

Further, more detailed roles are possible, as described in ISO standard ![ISO/IEC 20246]("https://www.iso.org/standard/67407.html").


### Review Types 

One of the main objectives of reviews is to uncover defects. All review types can aid in defect detection, and the selected review type should be based on the needs of the project, available resources, product type and risks, business domain, and company culture, among other selection criteria. The following lists the four most common types of reviews and their associated attributes.

**Informal review (e.g., buddy check, pairing, pair review)** 

- Main purpose: detecting potential defects 
- Possible additional purposes: generating new ideas or solutions, quickly solving minor problems 
- Not based on a formal (documented) process 
- May not involve a review meeting 
- May be performed by a colleague of the author (buddy check) or by more people 
- Results may be documented 
- Varies in usefulness depending on the reviewers 
- Use of checklists is optional 
- Very commonly used in Agile development

**Walkthrough**

- Main purposes: find defects, improve the software product, consider alternative implementations,
evaluate conformance to standards and specifications 
- Possible additional purposes: exchanging ideas about techniques or style variations, training of
participants, achieving consensus 
- Individual preparation before the review meeting is optional 
- Review meeting is typically led by the author of the work product 
- Scribe is mandatory 
- Use of checklists is optional 
- May take the form of scenarios, dry runs, or simulations 
- Potential defect logs and review reports are produced 
- May vary in practice from quite informal to very formal

**Technical review** 

- Main purposes: gaining consensus, detecting potential defects 
- Possible further purposes: evaluating quality and building confidence in the work product,
generating new ideas, motivating and enabling authors to improve future work products,
considering alternative implementations 
- Reviewers should be technical peers of the author, and technical experts in the same or other
disciplines 
- Individual preparation before the review meeting is required 
- Review meeting is optional, ideally led by a trained facilitator (typically not the author) 
- Scribe is mandatory, ideally not the author 
- Use of checklists is optional 
- Potential defect logs and review reports are produced 

**Inspection**

- Main purposes: detecting potential defects, evaluating quality and building confidence in the work
product, preventing future similar defects through author learning and root cause analysis 
- Possible further purposes: motivating and enabling authors to improve future work products and
the software development process, achieving consensus 
- Follows a defined process with formal documented outputs, based on rules and checklists 
- Uses clearly defined roles,  which are mandatory, and may include a dedicated reader 
- Individual preparation before the review meeting is required 
- Reviewers are either peers of the author or experts in other disciplines that are relevant to the
work product 
- Specified entry and exit criteria are used 
- Scribe is mandatory 
- Review meeting is led by a trained facilitator (not the author)
- Author cannot act as the review leader, reader, or scribe 
- Potential defect logs and review report are produced 
- Metrics are collected and used to improve the entire software development process, including the
inspection process 

