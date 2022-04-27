# What is Enclose
A simple, portable wrapper for various package managers (Currently in design stage).

## Purpose
To ease developing software from multiple environments (a.k.a multiple computers, OS's, etc) by
providing tools to install and manage heterogeneous dependencies effotlessly.

## Motivation
As software developers/enthusiasts/engineers/students/teachers, we like to create software tools to
automate tasks on different areas such as Data Processing, Systems Administration,
Document Typesetting, and, of course, Software Develpment itself. We also have a few (or a lot) bigger software
projects we work on for a living, for school or just for fun.

As such, different projects are implemented in different programming languages and each project has its own dependencies,
which are obtained from different sources such as:

- OS package repositories (apt, rpm)
- (More or less) programming language-specific repositories (cpan, pip, npm)
- Compiled from soure (github repos or tarballs)
- Other local dependencies (local git repos for our own projects)

(For the last two items the issue becomes recursive since tarballs or local projects in turn have their own
dependencies.)

Even though part of the code we write is used only by ourselves or by small teams, we like the fact that our software
just runs on the different machines we have at our disposal and it's even better if it works across OS's. However,
this is sometimes not easy to achieve given the dependency requirements.

Therefore, this proposal is to define a format for dependency specifications as simple as possible, and
a corresponding set of tools to interpret such specifications for automating dependency management as much
as possible without these tools needing difficult to install dependencies. To achieve this, we piggy-back on
existing package managers as much as we possibly can.



