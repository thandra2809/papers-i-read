# Summary: Using Reasoning about knowledge to analyze distributed systems

e ... this is really a long paper, just list the title and some abstract ...

## 1. Introduction

major complexities

- message delivery
- possible faulty
- unexpected behavior of processors (byzantine?)

> Recent work has shown these informal arguments can be completely formalized, using ideas for
formalizing knowledge that go back to work of philosophers in the late 1950s and early 1960s

> in this survey 0.0

Wide apply

> Thus the ideas presented apply perfectly well to the analysis of a system of communication robots, a bargaining session, or a conversation.
> interest in knowledge has been rising recently in such areas as distributed AI, economics, and linguistics

Possible Worlds model (Hintikka 1062)

- Besides the true state of affairs, an agent considers a number of other worlds or states of affairs possible
- An agent is said to know a fact \\fi if \\fi is true at all the worlds he considers possible
- The more worlds an agent considers possible, the greater her uncertainty, and the less she knows

- a run is a complete description of what happens in the system over time.  
- .... see highlight in pdf file

- everyone knows the knowledge
- everyone knows everyone knows the rules
  - reminds of a plot in friends, do they know we know that she knows
- recursive everyone knows f(n) = everyone knows f(n-1) f(1) = everyone knows fact \\fi

common knowledge is a prerequisite for simultaneous agreement and coordinated action.  

implicit knowledge -> deduce from existing knowledge

> if Alice knows that Bob is in love with either Carol or Susan,
and Charlie knows that Bob is not in love with Carol, then together
they implicitly know that Bob is in love with Susan, although neither Alice
nor Charlie individually has this knowledge.


## 2. The Possible Worlds Model

Need a language that allow us to express notions of knowledge in a straight way.

- agents 1,....,n
- primitive propositions
  - x = 0
  - process 3 is faulty
  - modal operations K1, ... Kn, K1\\fi 'agent 1 knows \\fi'
- Eg everyone in the group G knows
- Cg it is common knowledge among the agents in G
- Ig it is implicitly known among the agents in G

(a very fun language .... )

Kripke structure

- structure M for n agents is a tuple (S, n, J^l,..., JQ),
- can be viewed as a labeled directed graph

Formula

- could be true at one world but false at another

Three particular properties of the definition of knowledge

- agents know only true facts <- belief Although you may have false beliefs, you
cannot know something that is false.
- each agent knows all the logical consequences of his knowledge.
- an agent knows all valid formulas.

Does not take computation into account until Section 7.

## 3. Ascribing knowledge to processors in a distributed system

## 4. Common knowledge and the "Coordinated Attack" problem

## 5. Knowledge in asynchronous systems

## 6. Simultaneous byzantine agreement

## 7. Taking computation into account

## 8. Related work and future directions