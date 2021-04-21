# Black-box Test Techniques 


### Equivalence Partitioning

Equivalence partitioning divides data into partitions in such a way
that all the members of a given partition are expected to be processed in the same way (see Kaner 2013
and Jorgensen 2014). There are equivalence partitions for both valid and invalid values. 

- Valid values are values that should be accepted by the component or system. An equivalence
partition containing valid values is called a “valid equivalence partition.” 
- Invalid values are values that should be rejected by the component or system. An equivalence
partition containing invalid values is called an “invalid equivalence partition.” 
- Partitions can be identified for any data element related to the test object, including inputs,
outputs, internal values, time-related values (e.g., before or after an event) and for interface
parameters (e.g., integrated components being tested during integration testing). 
- Any partition may be divided into sub partitions if required. 
- Each value must belong to one and only one equivalence partition. 
- When invalid equivalence partitions are used in test cases, they should be tested individually, i.e.,
not combined with other invalid equivalence partitions, to ensure that failures are not masked.
Failures can be masked when several failures occur at the same time but only one is visible,
causing the other failures to be undetected.

To achieve 100% coverage with this technique, test cases must cover all identified partitions (including
invalid partitions) by using a minimum of one value from each partition. Coverage is measured as the
number of equivalence partitions tested by at least one value, divided by the total number of identified
equivalence partitions, normally expressed as a percentage. Equivalence partitioning is applicable at all
test levels. 

### Boundary Value Analysis

Boundary value analysis (BVA) is an extension of equivalence partitioning, but can only be used when the
partition is ordered, consisting of numeric or sequential data. The minimum and maximum values (or first
and last values) of a partition are its boundary values (see Beizer 1990).

For example, suppose an input field accepts a single integer value as an input, using a keypad to limit
inputs so that non-integer inputs are impossible. The valid range is from 1 to 5, inclusive. So, there are
three equivalence partitions: invalid (too low); valid; invalid (too high). For the valid equivalence partition,
the boundary values are 1 and 5. For the invalid (too high) partition, the boundary value is 6. For the
invalid (too low) partition, there is only one boundary value, 0, because this is a partition with only one
member.

In the example above, we identify two boundary values per boundary. The boundary between invalid (too
low) and valid gives the test values 0 and 1. The boundary between valid and invalid (too high) gives the
test values 5 and 6. Some variations of this technique identify three boundary values per boundary: the
values before, at, and just over the boundary. In the previous example, using three-point boundary
values, the lower boundary test values are 0, 1, and 2, and the upper boundary test values are 4, 5,
and 6 (see Jorgensen 2014).

Behavior at the boundaries of equivalence partitions is more likely to be incorrect than behavior within the
partitions. It is important to remember that both specified and implemented boundaries may be displaced
to positions above or below their intended positions, may be omitted altogether, or may be supplemented
with unwanted additional boundaries. Boundary value analysis and testing will reveal almost all such
defects by forcing the software to show behaviors from a partition other than the one to which the
boundary value should belong.

Boundary value analysis can be applied at all test levels. This technique is generally used to test
requirements that call for a range of numbers (including dates and times). Boundary coverage for a
partition is measured as the number of boundary values tested, divided by the total number of identified
boundary test values, normally expressed as a percentage. 

### Decision Table Testing

Decision tables are a good way to record complex business rules that a system must implement. When
creating decision tables, the tester identifies conditions (often inputs) and the resulting actions (often
outputs) of the system. These form the rows of the table, usually with the conditions at the top and the
actions at the bottom. Each column corresponds to a decision rule that defines a unique combination of
conditions which results in the execution of the actions associated with that rule. The values of the
conditions and actions are usually shown as Boolean values (true or false) or discrete values (e.g., red,
green, blue), but can also be numbers or ranges of numbers. These different types of conditions and
actions might be found together in the same table. The common notation in decision tables is as follows:

For conditions: 
- "Y" means the condition is true (may also be shown as T or 1) 
- "N" means the condition is false (may also be shown as F or 0) 
- "—" means the value of the condition doesn’t matter (may also be shown as N/A)

For actions: 

- X means the action should occur (may also be shown as Y or T or 1) 
- Blank means the action should not occur (may also be shown as – or N or F or 0)

A full decision table has enough columns (test cases) to cover every combination of conditions. By
deleting columns that do not affect the outcome, the number of test cases can decrease considerably. For
example by removing impossible combinations of conditions.

The common minimum coverage standard for decision table testing is to have at least one test case per
decision rule in the table. This typically involves covering all combinations of conditions. Coverage is
measured as the number of decision rules tested by at least one test case, divided by the total number of
decision rules, normally expressed as a percentage.

The strength of decision table testing is that it helps to identify all the important combinations of
conditions, some of which might otherwise be overlooked. It also helps in finding any gaps in the
requirements. It may be applied to all situations in which the behavior of the software depends on a
combination of conditions, at any test level. 

### State Transition Testing

Components or systems may respond differently to an event depending on current conditions or previous
history (e.g., the events that have occurred since the system was initialized). The previous history can be
summarized using the concept of states. A state transition diagram shows the possible software states,
as well as how the software enters, exits, and transitions between states. A transition is initiated by an
event (e.g., user input of a value into a field). The event results in a transition. The same event can result
in two or more different transitions from the same state. The state change may result in the software
taking an action (e.g., outputting a calculation or error message).

A state transition table shows all valid transitions and potentially invalid transitions between states, as well
as the events, and resulting actions for valid transitions. State transition diagrams normally show only the
valid transitions and exclude the invalid transitions.

Tests can be designed to cover a typical sequence of states, to exercise all states, to exercise every
transition, to exercise specific sequences of transitions, or to test invalid transitions.
State transition testing is used for menu-based applications and is widely used within the embedded
software industry. The technique is also suitable for modeling a business scenario having specific states
or for testing screen navigation. The concept of a state is abstract – it may represent a few lines of code
or an entire business process.

Coverage is commonly measured as the number of identified states or transitions tested, divided by the
total number of identified states or transitions in the test object, normally expressed as a percentage. For
more information on coverage criteria for state transition testing.

### Use Case Testing

Tests can be derived from use cases, which are a specific way of designing interactions with software
items. They incorporate requirements for the software functions. Use cases are associated with actors
(human users, external hardware, or other components or systems) and subjects (the component or
system to which the use case is applied).

Each use case specifies some behavior that a subject can perform in collaboration with one or more
actors (UML 2.5.1 2017). A use case can be described by interactions and activities, as well as
preconditions, postconditions and natural language where appropriate. Interactions between the actors
and the subject may result in changes to the state of the subject. Interactions may be represented
graphically by work flows, activity diagrams, or business process models.

A use case can include possible variations of its basic behavior, including exceptional behavior and error
handling (system response and recovery from programming, application and communication errors, e.g.,
resulting in an error message). Tests are designed to exercise the defined behaviors (basic, exceptional
or alternative, and error handling). Coverage can be measured by the number of use case behaviors
tested divided by the total number of use case behaviors, normally expressed as a percentage.

