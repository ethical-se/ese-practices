---
Scope: Single backlog item (epic or user story)
Phases: Any sprint/iteration (at start)
Roles: Agile team
Activities: Sprint/iteration planning meeting   
Abstraction/Refinement Level: Design and development 
---

Artifact: *Definition of Ready (Ethics-Enhanced)*
-------------------------------------------------
also known as INVEST+ Criteria (or INVVVEST or INV3EST)

> *Synopsis (taken from Agile Alliance Glossary): "As in the 'Definition of Done', in the Definition of Ready, the team makes explicit and visible the criteria (generally based on the INVEST matrix) that a user story must meet prior to being accepted into the upcoming iteration."*

A Definition of Ready (DoR) establishes the preconditions that must be met before a story can be taken off the backlog and included in a sprint. Its effort estimation (with story points) might or might not be included. 

This is an established Agile practice, enhanced and extended for ESE (this project/repository). See entry in [Agile Glossary](https://www.agilealliance.org/glossary/definition-of-ready/). 


### Motivation 

Being ready to move from analysis to design in a value-based approach, as defined in IEEE Std. 7000 and ESE, must be agreed upon.

#### Link to IEEE 7000

The Ethical Risk-Based Design Process (Clause 9) requires Value Requirements as input. The enhanced Definition of Ready verifies that such requirements exist. 

Also see mapping table in [Background Information](/ESE-BackgroundInformation.md).


### Template Structure and Notation(s)

Add the following criteria to the DoR checklist: 

1. Do the ConOps documentation and the Value Register have to be updated due to the outcome of the Story Valuation for this sprint/iteration and its backlog item set? Has this documentation work been added to the task backlog? 
2. Have one or more [EVRs](/ESE-Glossary.md#evr) and [VBSRs](/ESE-Glossary.md#vbsr) for the epic or the user story under consideration been elicited and documented? Do these requirements match the priorities of the values in the Value Register?
3. Do the INVEST criteria cover [ethical values](/ESE-Glossary.md#ethical-value) in addition to business and user value? 
4. Have negative consequences (potential harm) of realizing the epic or story been identified? 
5. Is a value-aware risk management and mitigation strategy in place?

ESE has a suggestive rather than normative character; it is ok to add context-specific criteria to this list.


### Example(s)

In the Lakeside Mutual example used in [Story Valuation](ESE-StoryValuation.md), the team created and uses the following DoR checklist: 

~~~
---
title: "ESE: Sample DoR Checklist"
author: Prowno Lakemutstaff
date: "mm, dd, yyyy (Project ESE)"
---

# Definition of Ready for "Custer Self Service" development at Lakeside Mutual 

## General DoR Questions

* [ ] Story is traceable to epic or business vision and project/product context information (Sprint 0)
* [ ] Story is estimated and meets INVEST criteria
* [ ] Acceptance test strategy and criteria have been defined
* [ ] Assumptions and risks are documented and required DevOps resources have been identified

## Value-Based Criteria: 

* [ ] ConOps documentation and the Value Register is up-to-date
* [ ] At least one EVR for the story has been elicited
* [ ] The INVEST criteria include/cover ethical value in addition to business/user value 
* [ ] Negative consequences (potential harm) have been identified and documented
* [ ] A risk mitigation strategy/tactic is in place and up-to-date 
~~~


### Tools

* Task management and issue-tracking tool
* Any virtual or physical tool for checklist processing
* [INVEST](https://www.agilealliance.org/glossary/invest/) matrix


### Hints and Pitfalls to Avoid

* Consistency matters; define and agree on a DoR at the project start. 
* Do not change the DoR during the project. If you do, it might yield false data and lose its value.
* Do not over-analyze. This would be anti-agile.
* Do no cheat. This would be unethical. Doing the right things and doing them right is a maxim that applies here (and elsewhere). <!-- redundant with DoD: Do not fall for the "checkbox ethics" antipattern. -->
* If you are not sure whether the DoR is met and decide to go ahead, document your doubts and be ready to go back if needed.


### Related Artifacts and Practices (incl. Alternatives)

In alphabetical order: 

* Acceptance Testing
* [Definition of Done](ESE-DefinitionOfDone.md)
* [Ethical Review](ESE-EthicalReview.md), performed at sprint/iteration end
* Product Backlog 
* [Value Retrospective](ESE-ValueRetrospective.md)
* Sprint Planning
* [Story Valuation](ESE-StoryValuation.md)
  

### More Information

* The Design Practice Repository/Reference (DPR) on [GitHub](https://github.com/socadk/design-practice-repository), on [LeanPub](https://leanpub.com/dpr) summarizes agile architecting practices such as user stories. 
* Wikpedia on [INVEST](https://en.wikipedia.org/wiki/INVEST_(mnemonic))
* ["New to agile? INVEST in good user stories"](https://agileforall.com/new-to-agile-invest-in-good-user-stories/) 


### Data Provenance 

```yaml
title: "ESE artifact: Ethics-Enabled DoR"
author: Olaf Zimmermann (ZIO)
date: "11, 13, 2023 (Version 1.0)"
copyright: The author, 2023-2024 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```