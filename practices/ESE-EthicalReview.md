---
Scope: Entire system, features added since last retrospective 
Phases: Analysis, design, implementation, test, maintenance 
Roles: Software engineer, value lead, other IEEE 7000 roles
Activities: Value-based systems engineering, validation and verification   
---

Activity and Artifact: *Ethical Review (Meeting and Report)*
------------------------------------------------------------
also known as Moral Value Reflection (Workshop and Notes)

### Goal and Purpose (Motivation)

Sprint reviews are essential Agile practices, the latter appearing in the [Agile Subway Map](https://www.agilealliance.org/agile101/subway-map-to-agile-practices/) maintained by the Agile Alliance. It seems natural to either ask questions about ethical values in these meetings — or run dedicated ones. The results of such efforts should be recorded:

> *An Ethical Review Report captures the results from an ethical values-enhanced (or -centric) sprint/project Ethical Review Meeting. It may include mere meeting notes and/or an assessment with follow up actions (aka recommendations and findings).*

Not performing an Ethical Review compromizes the value of ESE; the Story Valuation results must be taken into account during SOI construction, and the review checks that this has happened. 

### Instructions 
  
*Inspect the user story implementations with regards to the prioritized Value Cluster demonstrators and Value Requirements from Story Valuation in a meeting. Capture the meeting outcome in a report.*

Record answers to the following questions during the review meeting:

1. Have the [Ethical Value Requirements (EVRs)](/ESE-Glossary.md#evr) been included in the [acceptance testing](https://www.agilealliance.org/glossary/acceptance) and did these tests pass?
2. Has any feature been introduced that stands in conflict with the EVRs as well as the team's values and personal beliefs of each team member? If yes, have tradeoffs and mitigation tactics been discussed? 
3. Would all team members use the new features themselves, and also let their closest relatives use the new features (assuming that these individuals are in the target audience of the system under construction)? 
4. Have the behavior of the team and its members been in line with the eligible Codes of Conduct (CoCs), for instance the ["ACM Code of Ethics and Professional Conduct"](https://www.acm.org/code-of-ethics)? Does it respect the values of the involved organizations (sponsor, clients, business partners)?
5. Do any of the IEEE Std. and ESE artifacts (i.e., [ConOps](/ESE-Glossary.md#conops), [Value Register](/ESE-Glossary.md#value-register), EVRs) require further updates, caused by the review results?
  
There are no easy answers to many of these questions typically; this is inherent, discussing them (as well as follow-on questions) is as important as the outcome of this activity to create awareness, for instance when planning the next sprint/iteration.

#### Link to IEEE 7000

Regular reviews and retrospectives can be seen as the ESE realization of the Transparency Management Process in IEEE Std. 7000 (Clause 11).

### Notation(s)

The review results can be recorded in free form in a new text document or added to the reviewed artifacts.


### Example(s)

In the Lakeside Mutual example used in [Story Valuation](ESE-StoryValuation.md), the team reviews the IEEE Std. 7000 artifacts (ConOps, Value Register, EVRs, VBSRs) and the [design decisions](https://socadk.github.io/design-practice-repository/artifact-templates/DPR-ArchitecturalDecisionRecordYForm.html) made. Two sample Y-statements to be reviewed are:

~~~
ADR-01 
In the context of the Customer Self Service backend,
facing the need to satisfy EVR-1 and the resulting VBSR,
we decided for full CRUD in the Frontend-Backend Integration API 
and neglected other designs (such as wrappers)
to achieve the level 1 value "freedom"
accepting that opposing level 1 value "accountability" is harmed.
~~~ 

~~~
ADR-02 
In the context of the Customer Self Service backend,
facing the need to satisfy EVR-2 to EVR-3 and the resulting VBSR,
we decided for access control with OAuth2 and HTTPS 
to achieve the level 1 value "confidentiality"
accepting that opposing level 1 value "transparency" is somewhat harmed.
~~~ 

Note that this example is greatly simplified; HTTP and OAuth are not sufficient to satisfy all typical [Confidentiality, Integrity and Availability (CIA)](https://www.techtarget.com/whatis/definition/Confidentiality-integrity-and-availability-CIA) requirements. Role-Based Access Control (RBAC) as well as Attribute-Based Access Control (ABAC) and other security tactics on the implementation logic contribute to securing the application and its code.

Reviewing not only the ADRs but also their realization in design models and code, the team answers the five questions from above: 
  
* W.r.t EVR satisfaction (question 2), the team concludes that the H(igh) priority values Fairness and Privacy are respected in the implementation. Satisfying the EVR for the (M)edium priority value of Autonomy is still on the backlog, but the related feature has not been fully implemented yet.
* No new value conflicts arise (question 2). 
* Questions 3 and are all answered with "yes", and question 5 receives a "no" in this simple example.


### Tools

No specific tools are required. Wiki pages and/or templates in Word processors (e.g., Markdown and Pandoc) are suited to capture Ehtical Review results. 


### Usage (Produced and Consumed When)

Ethics Review reports result from Ethical Review meetings, which complement sprint review meetings. In line with the [Agile Manifesto](https://agilemanifesto.org/), face-to-face meetings are preferable over online/virtual meetings; meeting in a trusted, safe setting helps to be open and honest. 

Ethics Review reports can be archived to promote transparency and accountability (which, in turn, are ethical engineering values). They can also serve as additional context and requirements input for subsequent sprints/iterations and projects (or other product development efforts).


### Hints and Pitfalls to Avoid

The review can be run just like other ones, but extended with questions about values (see above):

* Review the valuated user stories that served as sprint/iteration input (with business, technical, ethical values to be considered). 
* Get all relevant stakeholders involved in the story valuation and ethics review, including end-user representatives. They know their values better than the development team. The ethical review is part of the conversation with them that Agile values call for.[^1] 
* Be honest: Do not schedule a review if you do not believe in its value. But document your rationale for the decision not to look back.
* Again, avoid checkbox ethics. 
* Apply techniques from other processes/methods as/if needed, for instance Proactive CARE and SoDIS (see [Literature](../ESE-Literature.md) for references). <!-- link to website https://ethics.acm.org/code-of-ethics/using-the-code/ -->

[^1]: To quote from the "Perfect 10" talk by Vaughn Vernon, the loudest and the longest talkers often cause harm ([read on](https://medium.com/olzzio/notes-from-the-architecture-and-modeling-learning-event-part-2-28287a7f13b0)). DO not interpret silence as agreement.


### Related Artifacts and Practices

In alphabetical order: 

* Acceptance Testing
* [Definition of Done](ESE-DefinitionOfDone.md), operating on epic/story level
* [Definition of Ready](ESE-DefinitionOfReady.md), also operating on epic/story level
* Product Backlog collecting/containing epics/stories and items 
* Sprint Planning, picking ready stories from backlog
* [Story Valuation](ESE-StoryValuation.md)
* [Value Retrospective](ESE-ValueRetrospective.md)  

### More Information

Miscellaneous: 

* The Design Practice Repository/Reference (DPR) on [GitHub](https://github.com/socadk/design-practice-repository), on [LeanPub](https://leanpub.com/dpr) summarizes agile architecting practices such as user stories. 
* An emerging [patterns](https://socadk.github.io/patterns/) repository curates pattern reading lists, for instance, one on [agile architecting and agile quality](https://socadk.github.io/patterns/reading-lists/agile-architecture.html). 
* An [Agile Glossary](https://www.agilealliance.org/agile101/agile-glossary/) is available on the Website of the Agile Alliance.
  

### Data Provenance 

```yaml
title: "ESE artifact: Ethics Review Meeting/Report"
author: Olaf Zimmermann (ZIO)
date: "11, 20, 2023 (Source: Project ESE)"
copyright: The author, 2023 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```