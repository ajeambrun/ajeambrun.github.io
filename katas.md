## Katas TDD/Clean Code/Refactoring

### Mob programming
In a first step for those topics, I mainly do coding kata with team using mob programing. I use the randori technic to be sure that every team member will have a chance to code.
First write a failing test, second make the test pass and write another failing test, etc

If done physically I use wireless keyboard and mouse on my own laptop so that developer don't lose time to setup a working new project on their own.
I don't know why, but it seems that creating a new Project is very often an issue for most of the dev I have seen in SG ;-(

Remotely I use the same Randori pace with a sync mechanism with a small shell script that push or pull automatically the code to/from github. Each developer have to launch this script so that they are always in sync. The one that have the keyboard share his screen

In a second step, I am trying to make the team do a refactoring in their own code base. I ask them to choose even part of a enhancement they have in their backlog, or a bugfix.

### FizzBuzz
It is often the first Kata I do with a team that want to improve on code quality
I use FizzBuzz kata to introduce TDD to teams. 
It is very simple so it helps to really explain the principles of the RGR loop.
I use it also to introduce Arrange Act Assert structure of a test method and what's behind the F.I.R.S.T. acronyme.

Sometimes if the team is still receptive after it, I introduce quickly the SOLID principles and ask the team to challenge
the produced code regarding those principles. I try to make them see that at least the O/C principle was violated during the coding session


### Roman To Arabic numerals Kata
This kata is very useful to feel the need of baby stepping. I am not using it very often, only if I have long time to coach the team  

### RPN Calculator
I use this kata to go deeper in the SOLID principles. 
This one fit very well the use of the strategy pattern to deal with the O/C principle.


### GildedRose
Very classical refactoring kata. I use it to introduce the concepts of safety harness. The use of the "approvals" framework (golden source test)
is a good temporary starting point to begin the work.
I ask the team to brainstorm about what they don't like or want to improve in the code. Then I make them pick and try to do a first one in the list. If it does not work I make them rollback the code and try another one.

I ask the team to go as far as possible in the refactoring before introducing the new feature.
I let them brianstorm about the choice between heritage and delegation. Both work for this one but if they choose heritage they have to deal with Liskov.
 
### Rental movies
Another classical refactoring kata. I use it only in a second phase.

### QuoteBot Kata
I don't know exactly from where this one come from. But I find it very interesting as it shows (a lot) issues of the dependecies (Dependencies Inversion).
Most of the work of this one is to break dependencies to be able to write tests. It helps introduce the concept of exploratory tests to sens the behavior of the code.
At the end it lead to an interesting design using the composite pattern.