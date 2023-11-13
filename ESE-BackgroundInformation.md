# Ethical Software Engineering (ESE) and IEEE Std. 7000

*Note:* Access to [IEEE Std. 7000](https://standards.ieee.org/ieee/24748-7000/11098/) is free after registration for IEEE Xplore (click on "Access via Subscription").

## Method (Processes, Concepts) Overview

IEEE Std. 7000 advises how to go from context to value to requirements to design:

![From Value to Requirements to Design](/images/ESE-ConceptsAndTraceRelations.png)

ADRs and Ethical Reviews are concepts from [DPR](https://socadk.github.io/design-practice-repository/activities/DPR-ArchitecturalDecisionCapturing.html) and ESE (this repository), respectively.


## Mappings between Agile Practices to Standards Concepts

See the [Glossary](ESE-Glossary.md) for brief summaries of IEEE Std. 7000 concepts and agile practices. All acronyms are defined there as well. 

### From Agile practices to IEEE Std. 7000 concepts

| Agile Practice | Related IEEE Std. 7000 Concept | Comments |
|-|-----------------------------------------------------|-|
| User Story (as Product Backlog Item) | Functional system requirement | see [ESE FAQs](/ESE-FAQ.md) |
| Sprint Planning | no direct mapping, parts of all processes executed in each iteration  | see ESE [FAQs](/ESE-FAQ.md) |
| Definition of Ready | [EVRs](/ESE-Glossary.md#evr) elicited (Clause 9) | V in INVEST widened |
| Definition of Done | Design artifacts produced and reviewed (Clause 10) | from Scrum, many templates/criteria |
| Sprint Review | Verification and validation activities in all processes | Novel practice in ESE: [Ethical Review](/practices/ESE-EthicalReview.md) |
| Retrospective | no direct mapping, contributes to Transparency Management Process | many variations |

The Scrum concept of [Product Vision](https://www.scrum.org/resources/what-product-vision) can also be mapped, to Clause 7 in particular, but also Clause 8 (the clauses are the chapters of the standard).

### From IEEE Std. 7000 processes to Agile practices

| IEEE Std. 7000 | Related Agile Practice  | Comments |
|-|-|-|
| Clause 7: Concept of Operations (ConOps)[^1] and Context Exploration Process [^2] | no direct pendant; epics as input | Concepts in HCI/UX community such as personas, Context Diagram in DPR |
| Clause 8: Ethical Values Elicitation and Prioritization Process | User Stories and related practices (e.g., [backlog refinement/grooming](https://www.agilealliance.org/glossary/backlog-refinement/)) | Novel practice in ESE: [Story Valuation](./practices/ESE-StoryValuation.md) |
| Clause 9: Ethical Requirements Definition Process | User Stories and related practices | Mapping, splitting; estimation/planning games such as [planning poker]() |
| Clause 10: Ethical Risk-Based Design Process | n/a (implicit, evolutionary/emerging) | Domain-Driven Design, "Just Enoughhttps://www.agilealliance.org/glossary/planning-poker/ Architecture" (related [patterns](https://socadk.github.io/patterns/reading-lists/agile-architecture.html)) |
| Clause 11: Transparency Management Process | no direct mapping | [Ethical Review Meeting/Report](./practices/ESE-EthicalReview.md), in ESE design decision logs from DPR |

[^1]: Note that the term "operations" in ConOps refers to the functioning of an application or system here; it is not to be confused with the Ops in DevOps and systems/service management (superset relation). IEEE Std. 7000 defines ConOps as "verbal and/or graphic statement, in broad outline, of an organization’s assumptions or intent in regard to an operation or series of operations" and then "The concept is designed to give an overall picture of the organization operations". ConOps has its roots in ISO/IEC/IEEE15288:2015.

[^2]: Several existing software engineering methods and tools emphasize context, for instance, the Domain-Driven Design tool [Context Mapper](https://contextmapper.org/) and architecture design methods such as those compiled in [Design Practice Repository/Reference (DPR)](https://socadk.github.io/design-practice-repository/). Event storming workshops yield domain model input and other analysis results; walking through an SOI started from an external business trigger may also contribute to ConOps creation and Context Exploration.

### From Agile Value and Practices to Ethical Values (and Back)

See [Frequently Asked Questions (FAQ)](/ESE-FAQ.md#agile-values-and-principles) page for the time being.


## Acknowledgment

This work was funded by the [Hasler Foundation](https://haslerstiftung.ch/en/welcome-to-the-hasler-foundation/).
