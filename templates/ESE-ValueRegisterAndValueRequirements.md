---
title: "ESE: Value Register"
author: NN
date: "mm, dd, yyyy (Source: Project NN)"
---

*Important note:* This is an early draft and preview, not ready for review and usage yet. It merely turns the section names from the standard into Markdown headings.

Artifact Template: *Value Register*
-----------------------------------
 
## Introduction

<!-- See Clauses 7 to 9 of IEEE Std. 7000. -->

## ConOps Reference

*Name and version of filled-out ConOps template*

## Values and Their Priorities

<!-- 
Page 44 in IEEE 7000:
"Identify one or more EVRs as socio-technology statements that describe possible risk treatment options that may promote and protect the prioritized core values and realize the value demonstrators. Treatment options are technical, organizational, or social.
NOTE—Each high-priority core value and value demonstrator has at least one EVR. Normally there are one or more EVRs for each core value. It is not necessary that for every identified value there is an EVR, the number of EVRs generated should reflect only high-priority items."

Page 45 in IEEE 7000: 
"Record each EVR with a unique reference number, its associated risks, prioritized core values, and related assumptions and constraints.
NOTE—A simple requirements register contains a table associating each EVR with one or more value clusters."
-->

#### Value Cluster Templates

a) Value Epic template:

~~~
As a [stakeholder role/group],
I value [core value],
as demonstrated in: 
- a realization of [related level 1 values]
- a reduction of [opposing level 1 values].
This value cluster has [H, M, L] priority for me. 
~~~

b) Value Weighting template: 

~~~
In the context of SOI [Name],
stakeholder [Role/Group] values [Value 1] more than [Value 2]
expecting benefits such as ...
running the risk of harms such as ...  
~~~

c) Value Narrative template:

~~~
When the SOI executes [epic user story/use case NN],
stakeholders expect it to promote, protect or create [values],
possibly degrading or prohibiting [values]
with the following externally observable and/or internally auditable behavior: [preconditions, postconditions]  
~~~

#### Standards Reference 
Annex G in IEEE Std. 7000 (which is suggestive, not normative) provides 12 examples of core/overarching valuesl.[^2]

| Overarching Value (Core) | Related Values (Themes) | Priority | Potential Conflicts (Opposing Values) | Story/Narrative/Demonstrator/Example |
|-|-|-|-|-|
| Autonomy | | H/M/L |  |  |
| Care |  | H/M/L |  | |
| Control |  | H/M/L | | |
| Fairness |  | H/M/L | | |
| Inclusiveness |  | H/M/L | | |
| Innovation |  | H/M/L | | |
| Perfection |  | H/M/L | | |
| Privacy |  | H/M/L | | |
| Respect |  | H/M/L | | |
| Sustainability |  | H/M/L | | |
| Transparency |  | H/M/L | | |
| Trust | | H/M/L | | |
| *additional value n* | | H/M/L | | |
| ... | | H/M/L | | |

[^2]: For example, note that Accountability is not listed as a top-level value in Annex G but is mentioned several times in IEEE Std. 7000. 

## EVRs

Enhanced User Story template:

~~~
As a [role]
I want to [action/feature]
so that [benefit] is achieved 
  and that [Values a, b, c] are promoted,
  accepting that [Values x, y, z] are reduced.
~~~

### EVR-nn

<!-- 

Page 44 in IEEE 7000:
"Identify one or more EVRs as socio-technology statements that describe possible risk treatment options that may promote and protect the prioritized core values and realize the value demonstrators. Treatment options are technical, organizational, or social.
NOTE—Each high-priority core value and value demonstrator has at least one EVR. Normally there are one or more EVRs for each core value. It is not necessary that for every identified value there is an EVR, the number of EVRs generated should reflect only high-priority items."

Page 45 in IEEE 7000: 
"Record each EVR with a unique reference number, its associated risks, prioritized core values, and related assumptions and constraints.
NOTE—A simple requirements register contains a table associating each EVR with one or more value clusters."
-->

*Value register reference*

*Risk and their treatment(s)*

*Assumptions and constraints*


## VBSRs (optional in ESE)

Template (extended user story format):

<!-- 
SEI/Agile Quality Scenario Template:

|Topic | Value|
|-|-|
|*Source*| ... |
|*Stimulus*| ... |
|*Environment*| ... |
|*Artifact*| ... |
|*Response*| ... |
|*Response Measure*| ... |
-->

Value Quality Scenario template:

| Scenario Element | ESE Usage of Element |
|-|-|
| *Stimulus* | Epic or user story or component of SOI; Value Register entry and/or EVR as response |
| *Concern Of (Source)* | Stakeholder as stimulus source |
| *Observable When* | Environment (e.g., from ConOps) |
| *Materializing In* | Artifact such as design element xyz in the [SOI](/ESE-Glossary.md/#soi) |
| *Value Requirement/Response* | Observable behavior after stimulus, in envirinment and artifact |
| *Value Requirement/Response Measure* | Quantification of observable behavior after stimulus |

Story/ADRish template for VBSRs:

VBSR-m [name]:
To satisfy [EVR-n] and treat the risks related to it,
a H/M/L priority concern of [stakeholder name, individual role or group],
 * the SOI has to implement technical risk treatment option ... (and/or)
 * the organization developing and operating the SOI has to ... (and/or)
 * the following social construct(s) will have to be realized ...


## Open Issues and Decisions Made

*Decision backlog and record.*
