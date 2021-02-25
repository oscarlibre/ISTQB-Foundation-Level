
# Seven Testing Principles

### 1. Testing shows the presence of defects, not their absence

- Testing can show that defects are present, but cannot prove that there are no defects. 

- Testing reduces the probability of undiscovered defects remaining in the software 

- Even if no defects are found, testing is not a proof of correctness

<hr/>

### 2. Exhaustive testing is impossible

- Testing everything (all combinations of inputs and preconditions) is not feasible except for trivial cases

- Rather than attempting to test exhaustively, risk analysis, test techniques, and priorities should be used to
focus test efforts

 <hr/>
 
### 3. Early testing saves time and money

![](https://s7280.pcdn.co/wp-content/uploads/2017/07/key-2.png)

- To find defects early, both static and dynamic test activities should be started as early as possible in the
software development lifecycle. 

- Testing early in the software development lifecycle helps reduce or eliminate costly changes 

- Early testing is sometimes referred to as shift left. 

<hr/>

### 4. Defects cluster together  

- Bugs are not often distributed evenly throughout an application

- A small number of modules usually contains most of the defects discovered during pre-release testing, or
is responsible for most of the operational failures. 

- Predicted defect clusters, and the actual observed defect clusters in test or operation, are an important
 input into a risk analysis used to focus the test effort
 
 <hr/>
 
### 5. Beware of the pesticide paradox 

- If the same tests are repeated over and over again, eventually these tests no longer find any new defects.

- To detect new defects, existing tests and test data may need changing, and new tests may need to be
written. 

- In some cases, such as automated regression testing, the pesticide paradox has a
beneficial outcome, which is the relatively low number of regression defects

<hr/>

### 6. Testing is context dependent 

- Testing is done differently in different contexts.For example, safety-critical industrial control software is
tested differently from an e-commerce mobile app. 

- What you are testing will always affect your approach 

<hr/>

### 7. Absence-of-errors is a fallacy

- It's impossible that testers can run all possible tests and find all possible defects (principles 1 and 2)

- it is a fallacy to expect that just finding and fixing a large number of defects will ensure the success of a system

