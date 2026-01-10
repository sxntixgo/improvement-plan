# Track 11: JavaScript/Node.js

**Duration:** 20 weeks | **Hours/week:** 18 | **Priority:** MEDIUM
**Goal:** Full-stack JS for security tooling

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Phase Overview

|Phase|Weeks|Focus                  |
|-----|-----|-----------------------|
|1    |46-53|JavaScript Fundamentals|
|2    |54-57|Node.js & Express      |
|3    |58-61|Advanced Patterns      |
|4    |62-65|Security Focus         |

-----

## Books You Already Own

|Book                                         |Type          |
|---------------------------------------------|--------------|
|Node.js: The Comprehensive Guide (Springer)  |Reference     |
|Web Development with Node and Express (Brown)|Project-driven|
|You Don't Know JS 1st edition (Simpson)      |Deep dive     |
|Eloquent JavaScript (Haverbeke)              |Project-driven|

-----

## Books to Consider

|Book                                      |Cost   |Project-Driven? |
|------------------------------------------|-------|----------------|
|YDKJSY: Scope & Closures 2nd ed (optional)|~$15-20|❌ No (deep dive)|
|Node.js Design Patterns                   |~$40   |✅ Yes (patterns)|

**Note on YDKJSY 2nd Edition:**

- Only 2 published: *Get Started* and *Scope & Closures*
- 2 drafts (readable but unedited): *Objects & Classes*, *Types & Grammar*
- 2 canceled: *Sync & Async*, *ES.Next & Beyond*
- You own 1st edition, so only *Scope & Closures* 2nd ed is worth buying

-----

## Free Resources

|Resource             |URL                               |Type              |
|---------------------|----------------------------------|------------------|
|Eloquent JavaScript  |eloquentjavascript.net            |Project-driven    |
|YDKJS/YDKJSY (GitHub)|github.com/getify/You-Dont-Know-JS|Deep dive         |
|JavaScript30         |javascript30.com                  |Projects (30 days)|
|Namaste JavaScript   |YouTube                           |Video course      |

-----

## Phase 1: JavaScript Fundamentals (Weeks 46-53)

**Primary Resource:** Eloquent JavaScript (project-driven, matches your learning style)

|Week|Chapters|Focus                                  |
|----|--------|---------------------------------------|
|46  |1-3     |Values, program structure, functions   |
|47  |4-5     |Data structures, higher-order functions|
|48  |6-7     |Objects, project: robot                |
|49  |8-9     |Bugs/errors, regex                     |
|50  |10-11   |Modules, async programming             |
|51  |12-13   |Project: programming language          |
|52  |14-15   |Browser, DOM                           |
|53  |16-18   |Events, project: platform game         |

**Supplement:** JavaScript30 challenges alongside reading

-----

## Phase 2: Node.js & Express (Weeks 54-57)

**Primary Resource:** Web Development with Node and Express (Brown) - Already owned

|Week|Focus                             |
|----|----------------------------------|
|54  |Node.js basics, npm, modules      |
|55  |Express setup, routing, middleware|
|56  |Templating, forms, sessions       |
|57  |REST APIs, authentication         |

**Reference:** Node.js: The Comprehensive Guide (Springer)

-----

## Phase 3: Advanced Patterns (Weeks 58-61)

|Week|Focus                |Resource                         |
|----|---------------------|---------------------------------|
|58  |Event loop deep dive |YDKJS 1st ed: Async & Performance|
|59  |Design patterns      |Node.js Design Patterns          |
|60  |Streams, buffers     |Springer book chapters           |
|61  |Testing (Jest, Mocha)|Hands-on                         |

-----

## Phase 4: Security Focus (Weeks 62-65)

|Week|Focus                                 |
|----|--------------------------------------|
|62  |Node.js security best practices       |
|63  |OWASP Node.js cheatsheet              |
|64  |Prototype pollution, injection attacks|
|65  |Security code review practice         |

-----

## Projects & Outputs

|Project               |Output                 |Share    |
|----------------------|-----------------------|---------|
|Todo App              |Basic CRUD with Express|GitHub   |
|URL Shortener         |REST API practice      |GitHub   |
|JS Security Cheatsheet|Personal reference doc |Blog post|

-----

## JavaScript Code Review Checklist

- [ ] Prototype pollution vectors?
- [ ] eval() or Function() usage?
- [ ] child_process with unsanitized input?
- [ ] JSON.parse on untrusted input?
- [ ] Missing input validation?
- [ ] Hardcoded secrets?
- [ ] DOM-based XSS sources/sinks?
- [ ] Proper async/await (no unhandled promises)?
- [ ] Event loop blocking?

-----

## Checkpoint

You should be able to build full-stack Node.js applications and conduct JS security reviews.
