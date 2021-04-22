# White-box Test Techniques

White-box testing is based on the internal structure of the test object. White-box test techniques can be
used at all test levels, but the two code-related techniques discussed in this section are most commonly
used at the component test level.


### Statement Testing and Coverage 

Statement testing exercises the potential executable statements in the code. Coverage is measured as
the number of statements executed by the tests divided by the total number of executable statements in
the test object, normally expressed as a percentage. 


### Decision Testing and Coverage 

Decision testing exercises the decisions in the code and tests the code that is executed based on the
decision outcomes. To do this, the test cases follow the control flows that occur from a decision point
(e.g., for an IF statement, one for the true outcome and one for the false outcome; for a CASE statement,
test cases would be required for all the possible outcomes, including the default outcome).
Coverage is measured as the number of decision outcomes executed by the tests divided by the total
number of decision outcomes in the test object, normally expressed as a percentage. 


### The Value of Statement and Decision Testing 

When 100% statement coverage is achieved, it ensures that all executable statements in the code have
been tested at least once, but it does not ensure that all decision logic has been tested. Statement testing 
may provide less coverage than decision testing.

When 100% decision coverage is achieved, it executes all decision outcomes, which includes testing the
true outcome and also the false outcome, even when there is no explicit false statement (e.g., in the case
of an IF statement without an else in the code). Statement coverage helps to find defects in code that was
not exercised by other tests. Decision coverage helps to find defects in code where other tests have not
taken both true and false outcomes.

Achieving 100% decision coverage guarantees 100% statement coverage (but not vice versa)
