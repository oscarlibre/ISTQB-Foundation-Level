#  Software Development Lifecycle Models

A software development lifecycle model describes the types of activity performed at each stage in a
software development project, and how the activities relate to one another logically and chronologically.
There are a number of different software development lifecycle models, each of which requires different
approaches to testing. 

### Software Development and Software Testing 

In any software development lifecycle model, there are several characteristics of good testing: 

- For every development activity, there is a corresponding test activity 
- Each test level has test objectives specific to that level 
- Test analysis and design for a given test level begin during the corresponding development activity 
- Testers participate in discussions to define and refine requirements and design, and are involved
in reviewing work products as soon as drafts are available 

---
**NOTE**

No matter which software development lifecycle model is chosen, test activities should start in the early
stages of the lifecycle, adhering to the testing principle of early testing. 

---

The two common software development lifecycle model groups are the following:

**Sequential development models:**  The software development process is linear, sequential flow
of activities (any phase begins when the previous phase is complete). In theory, there is no overlap of phases, 
but in practice, it is beneficial to have early feedback from the following phase. Sequential development models deliver 
software that contains the complete set of features, but typically require months or years for delivery to stakeholders and users. 
Some of popular models of this group are:

- *Waterfall model:* Here the development activities (e.g., requirements analysis, design, coding, testing)
are completed one after another. In this model, test activities only occur after all other development
activities have been completed.
- *V-model:* It integrates the test process throughout the development process, implementing the principle of early testing. Further, it includes test levels associated with each corresponding development phase, which further supports early testing . In this model, 
the execution of tests associated with each test level proceeds sequentially, but in some cases overlapping occurs.


**Iterative and incremental development models**: Components or systems developed using these methods often involve overlapping and iterating test
levels throughout development. Ideally, each feature is tested at several test levels as it moves towards delivery. In some cases, teams use continuous
delivery or continuous deployment, both of which involve significant automation of multiple test levels as part of their delivery pipelines. 
Many development efforts using these methods also include the concept of self-organizing teams, which can change the way testing work is organized as well
as the relationship between testers and developers. These methods form a growing system, which may be released to end-users on a feature-by-feature
basis, on an iteration-by-iteration basis, or in a more traditional major-release fashion. Regardless of whether the software increments are released to end-users, regression testing is increasingly important
as the system grows. In contrast to sequential models, iterative and incremental models may deliver usable software in weeks or even days, but may only 
deliver the complete set of requirements product over a period of months or even years

- *Incremental development model:* It involves establishing requirements, designing, building, and testing a system in
pieces, which means that the software’s features grow incrementally. The size of these feature increments
varies, with some methods having larger pieces and some smaller pieces. The feature increments can be
as small as a single change to a user interface screen or new query option. 

- *Iterative development model:* It occurs when groups of features are specified, designed, built, and tested together in a series of cycles, 
often of a fixed duration. Iterations may involve changes to features developed in earlier iterations, along with changes in project scope. 
Each iteration delivers working software which is a growing subset of the overall set of features until 
the final software is delivered or development is stopped. Examples include: 
    - Rational Unified Process: Each iteration tends to be relatively long (e.g., two to three months),
and the feature increments are correspondingly large, such as two or three groups of related
features 
    - Scrum: Each iteration tends to be relatively short (e.g., hours, days, or a few weeks), and the
feature increments are correspondingly small, such as a few enhancements and/or two or three
new features 
    - Kanban: Implemented with or without fixed-length iterations, which can deliver either a single
enhancement or feature upon completion, or can group features together to release at once 
    - Spiral: Involves creating experimental increments, some of which may be heavily re-worked or
even abandoned in subsequent development work 

### Software Development Lifecycle Models in Context 

- Software development lifecycle models must be selected and adapted to the context of project and product characteristics. 
- An appropriate software development lifecycle model should be selected and adapted based on the project goal, the type of product being developed, business priorities and identified product and project risks (e.g an administrative system is different of a safety-critical system). 
- Depending on the context of the project, it may be necessary to combine or reorganize test levels and/or test activities. 
- Software development lifecycle models themselves may be combined, for example IoT systems, which consist of many different objects, such as devices, products, and services, typically apply separate software development lifecycle models for each object. 


