---
layout: page
title: Coding Notes
description: to learn
---



A pure function is a function where the return value is only determined by its input values, without observable side effects. This is how functions in math work: Math.cos(x) will, for the same value of x, always return the same result. Computing it does not change x. It does not write to log files, do network requests, ask for user input, or change program state. It’s a coffee grinder: beans go in, powder comes out, end of story.


Replication - Copying an entire table or database onto multiple servers. Used for improving speed of access to reference records such as master data.

Partitioning - Splitting up a large monolithic database into multiple smaller databases based on data cohesion. Example - splitting a large ERP database into modular databases like accounts database, sales database, materials database etc.

Clustering - Using multiple application servers to access the same database. Used for computation intensive, parallelized, analytical applications that work on non volatile data.

Sharding - Splitting up a large table of data horizontally i.e. row-wise. A table containing 100s of millions of rows may be split into multiple tables containing 1 million rows each. Each of the tables resulting from the split will be placed into a separate database/server. Sharding is done to spread load and improve access speed. Facebook/twitter tables fit into this category.