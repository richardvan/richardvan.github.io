---
layout: page
title: Coding Notes
description: to learn
---

## Software Engineering Principles
*Casablanca: "The fundamental things apply, as time goes by."*

### Software Project Approach
1. Think through the problem completely before any attempts at implementing (coding)
2. Plan incremental development from high level down approach

### Software Engineering Principles

1. Don't Repeat Yourself (**DRY**) Principle
  * Every piece of knowledge must have one authentic unambiguous representation
  * DRYness achieved by good planning
  * Goal is to reduce complexity by dividing project into manageable components
  * vs WET - *write everything twice*, *waste everyone's time*
2. Keep It Simple Stupid (**KISS**) Principle
  * Strive for simplest way of doing something
  * Identifies three alerts when looking at requirements
    *1 functionality with bad cost/benefit ratio
    *2 functionality highly dependent on others
    *3 functionality likely to grow in complexity
3. You Ain't Gonna Need It (**YAGNI**)
  * If it's not in the concept, it's not in the code
  * Reduce complexity by reducing the number of components
  * Strive for simplicity by not implementing anything at all

### Software Project Goal
1. Make it WORK first - get the environment built, think artist drawing something left to right, need scaffolding
2. Make it work RIGHT - given inputs and expected outputs should work and be tested
3. THEN look pretty - refactoring code, nice comments,

#### Useful links:
http://code.tutsplus.com/tutorials/3-key-software-principles-you-must-understand--net-25161
https://www.vikingcodeschool.com/software-engineering-basics/basic-principles-of-software-engineering

Good video explaining roots and evolution of software engineering in real world terms:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=9IPn5Gk_OiM
" target="_blank"><img src="http://img.youtube.com/vi/9IPn5Gk_OiM/0.jpg" 
alt="Software Engineering, Barcelona Ruby Conference" width="240" height="180" border="10" /></a>

---

## Design Patterns

### Singleton

Only one object instance of a class initiated at any given time. There is a cardinality of one.

### Dependency Injection

Seperate initialization from business logic, the responsibility is outsourced to another class or framework from your code.


### Module Pattern

Mimic conventional software engineering by having object-oriented static members. Provides way to wrap public and private members to the world outside of the module.  Allows for aster namespace resolution, avoid collission of methods/variables in other global APIs, cleaner code.

http://www.adequatelygood.com/JavaScript-Module-Pattern-In-Depth.html
http://viralpatel.net/blogs/javascript-module-pattern/


### Factory Pattern

Your code is responsible for creating objects without needing to know the concrete types.


---


### Testing related

A pure function is a function where the return value is only determined by its input values, without observable side effects. This is how functions in math work: Math.cos(x) will, for the same value of x, always return the same result. Computing it does not change x. It does not write to log files, do network requests, ask for user input, or change program state. It’s a coffee grinder: beans go in, powder comes out, end of story.

---

### Backend Related stuff


Replication - Copying an entire table or database onto multiple servers. Used for improving speed of access to reference records such as master data.

Partitioning - Splitting up a large monolithic database into multiple smaller databases based on data cohesion. Example - splitting a large ERP database into modular databases like accounts database, sales database, materials database etc.

Clustering - Using multiple application servers to access the same database. Used for computation intensive, parallelized, analytical applications that work on non volatile data.

Sharding - Splitting up a large table of data horizontally i.e. row-wise. A table containing 100s of millions of rows may be split into multiple tables containing 1 million rows each. Each of the tables resulting from the split will be placed into a separate database/server. Sharding is done to spread load and improve access speed. Facebook/twitter tables fit into this category.