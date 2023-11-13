---
Scope: Single backlog item (epic or user story)
Phases: Any sprint/iteration (end of it)
Roles: Agile team
Activities: Sprint/iteration review meeting  
Abstraction/Refinement Level: Design and development
---

Artifact: *Definition of Done (Ethics-Enhanced)*
------------------------------------------------
also known as Done-Done

> *Synopsis (taken from Agile Alliance Glossary): "The team agrees on, and displays prominently somewhere in the team room, a list of criteria which must be met before a product increment 'often a user story' is considered 'done'. Failure to meet these criteria at the end of a sprint normally implies that the work should not be counted toward that sprint’s velocity."*

A Definition of Done (DoD) is the base for sprint/iteration planning and progress tracking (e.g., via velocity metrics and burndown charts). It also serves as a document of understanding when changes are welcome and when they are not. It typically contains criteria such as such as product owner approval obtained, unit test written and passed, demo to end user given, documentation including example written and reviewed, code and other artifacts reviewed by at least one non-author.

Maintaining a DoD is an established Agile practice, enhanced and extended for ESE (this project/repository). 


### Motivation 

See entry in [Agile Glossary](https://www.agilealliance.org/glossary/definition-of-done/) for general motivation. 

The completion of a step in the value-based approach in IEEE Std. 7000 and Story Valuation in ESE also must be agreed upon.


#### Link to IEEE 7000

The DoD is checked when the results of the Ethical Risk-Based Design Process (Clause 9) have been implemented. 

Also refer to the process mapping tables on the [Background Information](/ESE-BackgroundInformation.md#from-agile-practices-to-ieee-std-7000-concepts) page.


### Template Structure and Notation(s)

Add the following criteria to your already existing DoD checklist: 

* Have the IEEE Std. 7000 artifacts ([ConOps](/ESE-Glossary.md#conops) documentation, the Value Register, [EVRs](/ESE-Glossary.md#evr)/[VBSRs](/ESE-Glossary.md#vbsr)) been updated for accuracy and completeness? 
* Does the chosen design satisfy the EVRs and VBSRs as desired? 
* Are all made design decisions sound w.r.t. business requirements as well as EVRs and VBSRs (and their priorities)? Can they be traced back to requirements? Are the conflicts and tradeoffs made explicit? 
* Will the overall design work in practice (in terms of technical feasibility and user acceptance)? Have all new design elements been validated and verified in that regard? 
* Have all design decisions and design updates been documented so that the IEEE Std. 7000 Transparency Management Process can pick them up? For instance, have the decisions been recorded in a recognized ADR format<!-- example: [MADR](https://github.com/adr/madr/blob/main/template/adr-template.md)-->?

ESE has a suggestive rather than normative character; it is ok to add context-specific criteria to this list.


### Example(s)

In the Lakeside Mutual example used in [Story Valuation](ESE-StoryValuation.md), the team created and uses the following DoD checklist: 

~~~
---
title: "ESE: Sample DoD Checklist"
author: Prowno Lakemutstaff
date: "mm, dd, yyyy (Source: Project ESE)"
---

# Definition of Done for "Custer Self Service" development at Lakeside Mutual 

## General DoD Questions

* [ ] Automated build is green
* [ ] Minimum viable documentation is available
* [ ] End user test has been performed and succeeded
* [ ] Product manager/owner has signed completion of story off 
* [ ] to be continued

## Value-Based Done Criteria: 

* [ ] ConOps documentation, the Value Register and the EVRs have been reviewed for accuracy and completeness
      These ESE/IEEE Std. 7000 artifacts are up to date.
* [ ] The design satisfies the EVRs. 
* [ ] The chosen designs/the made decisions are sound and can be traced back to requirements
* [ ] There is evidence that the design will work in practice/production; its implementation has been validated and verified.
* [ ] All design updates been documented and are ready for the Transparency Management Process to pick them up? 
~~~


### Tools

* Task management and issue-tracking tool
* Any virtual or physical tool for checklist processing
* Reusable DoD criteria templates and catalogs 


### Hints and Pitfalls to Avoid

* Consistency matters; define and agree on a DoD at the project start and stick to it. Do not change the criteria in flight. Otherwise, the practice might yield false data and lose its value.
* Plan and execute the [acceptance testing](https://www.agilealliance.org/glossary/acceptance) adequately. Keep an eye on effort vs. benefit; it might not be needed and/or not possible to let end users test every story in each sprint. Choosing a suited granularity and frequency is a product management responsibility.
* Be honest in your assessments.[^1] 
  
[^1]: Arguably, honesty is a fundamental ethical value that can be expected to also appear in many Value Registers.


### Related Artifacts and Practices 

In alphabetical order: 

* Acceptance Testing
* [Definition of Ready](ESE-DefinitionOfReady.md)
* [Ethical Review](ESE-EthicalReview.md), performed at sprint/iteration end (all "done" stories)
* Product Backlog 
* [Value Retrospective](ESE-ValueRetrospective.md)
* Sprint Planning
* [Story Valuation](ESE-StoryValuation.md)
  

### More Information

Annex I of IEEE Std. 7000 suggests structure and content of a complete Case for Ethics; the DoD definition can be part of it.

The Design Practice Repository/Reference (DPR) on [GitHub](https://github.com/socadk/design-practice-repository) and on [LeanPub](https://leanpub.com/dpr) summarizes agile architecting practices such as user stories.

["Enhancing Your "Definition of Done" Can Improve Your Minimum Viable Architecture "](https://www.infoq.com/articles/definition-of-done-mva/) on InfoQ suggests architectural extensions to the DoD. There is a [DoD for architectural decisions](https://medium.com/olzzio/a-definition-of-done-for-architectural-decisions-426cf5a952b9) as well.


### Data Provenance 

```yaml
title: "ESE artifact: Ethics-Enabled DoD"
author: Olaf Zimmermann (ZIO)
date: "11, 13, 2023 (Source: Project ESE)"
copyright: The author, 2023 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```
