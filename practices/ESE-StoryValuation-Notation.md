---
Scope: Larger unit (epic) or single feature/capability (story)
Phases: Product vision/upfront analysis and design; each sprint/iteration
Roles: Software engineer; product manager, user advocate, value lead
Input: Project goals and vision, business requirements, technical requirements; ConOps, (optional) existing Value Register
Output: New or updated Value Register, EVRs, (optional) VBSRs
---

Notations for Activity: [*Story Valuation*](/practices/ESE-StoryValuation.md)
-----------------------------------------

### Notation(s)

When following the above instructions to achieve the goal and purpose of Story Valuation, notations and/or text templates are required to record intermediate and final results; method techniques yielding such results are featured in [here](/practices/ESE-StoryValuation.md#valuation-techniques).

#### Value Register
ESE does not *mandate* any particular format for the IEEE Std. 7000 Value Register; overview figures and comparison tables can be well suited. We still *suggest* three novel formats here: Value Epic, Value Weighting and Value Narrative. 

a) *Value Epic* is the first proposed notation template:

~~~
As a [stakeholder role/group],
I value [core value],
as demonstrated in: 
- a realization of [related level 1 values]
- a reduction of [opposing level 1 values].
This value cluster has [H, M, L] priority for me. 
~~~

Values can be positive or negative in a given context; IEEE Std. 7000 explains that in Annex "B.3 Value axioms" (so absence of certain values, the negative ones, is good!). The wording in the template is inspired by the definition of terms in the standard. <!-- also used: "creation" and "prohibition" -->

b) Complementary and/or alternatively, a relative *Value Weighting* makes a consideration/assessment explicit. It may look like this:

~~~
In the context of SOI [Name],
stakeholder [Role/Group] values [Value 1] more than [Value 2]
expecting benefits such as ...
running the risk of harms such as ...  
~~~

Again, please note that the words [benefit](/ESE-Glossary.md#benefit) and [harm](/ESE-Glossary.md#harm) do not imply the usage, or sole usage, of any particular ethical theory here.  

c) The third proposal, *Value Narrative*, links values to system behavior:

~~~
When the SOI executes [epic user story/use case NN],
stakeholders expect it to promote, protect or create [values],
possibly degrading or prohibiting [values]
with the following externally observable and/or internally auditable behavior: [preconditions, postconditions]  
~~~

Collectively, the value epics, weightings, narratives comprise the Value Register for a SOI (or, picking up an agile term, the value backlog). See sections on techniques and examples for additional examples. 

***Disclaimer:*** Please view these proposed notations as intermdiate drafts, serving as invitations to a continued method engineering discussion. [Examples](/practices/ESE-StoryValuation.md#examples) are available.

#### Ethical Value Requirement (EVRs)
As an important type of non-functional requirements, [EVRs](/ESE-Glossary.md#evr) can be written up either in free form or in a structured way. IEEE Std. 7000 specifies how to document Values and EVRs in a rather elaborate form; or details, please refer to pages 40 to 42 in Clause 8 (Values) and then pages 44 to 46 (EVRs) in Clause 9 of the standard. 

<!-- IEEE Std. 7000: 
"NOTE 1—EVRs can be expressed in formal requirement statements, use cases, user stories, scenarios, or other forms." 
"NOTE 2—EVRs can be used to translate the prioritized core values into the system’s value dispositions."

"socio-technology statements that describe possible risk treatment options that may promote and protect the prioritized core values and realize the value demonstrators. Treatment options are technical, organizational, or social." [...] "Record each EVR with a unique reference number, its associated risks, prioritized core values, and related assumptions and constraints."
-->

IEEE Std. 7000 gives an example of an EVR in the full-body scanner SOI in B.2: "The system shall protect the privacy of body images of scanned passengers.". The standard talks about "risk treatment options" (which are technical, organizational, social) and "value demonstrator realization". In ESE, we see these information elements at the interface/intersection between analysis and design.  

The writeup of value requirements should pass the [SMART NFR](https://socadk.github.io/design-practice-repository/activities/DPR-SMART-NFR-Elicitation.html) test for non-functional requirements; making them context-specific (in terms of features or components) and measurable (so that they can be verified/tested) is particularly important.

In ESE, EVRs may take the standard story form, slightly extended with a brief ethical value assessment:

~~~
As a [role]
I want to [action/feature]
so that [benefit] is achieved 
  and that [values a, b, c] are promoted,
  accepting that [values x, y, z] are reduced.
~~~

Alternatively, the value-enhanced user story may also refer to Value Register entries, possibly expressed as Value Epics, Value Weightings and/or Value Narratives (as introduced previously). Note that risk treatment options and value demonstrators are not made explicit in this template; such information can be added in free form.
 
#### Value-Based System Requirement (VBSRs)

a) VBSRs may adopt the Quality Attribute Scenario (QAS) table format from the SEI ([introduction](https://socadk.github.io/design-practice-repository/artifact-templates/DPR-QualityAttributeScenario.html) with examples, [online article](https://www.codementor.io/@antoniopfesilva/how-to-write-meaningful-quality-attributes-for-software-development-ez8y90wyo) with more examples, [arc42 Quality Model](https://quality.arc42.org) with even more examples): 

| Scenario Element | ESE Usage of Element |
|-|-|
| *Stimulus* | Epic or user story or component of SOI; Value Register entry and/or EVR as response |
| *Concern Of (Source)* | Stakeholder as stimulus source |
| *Observable When* | Environment (e.g., from ConOps) |
| *Materializing In* | Artifact such as design element xyz in the [SOI](/ESE-Glossary.md/#soi) |
| *Value Requirement/Response* | Observable behavior after stimulus, in envirinment and artifact |
| *Value Requirement/Response Measure* | Quantification of observable behavior after stimulus |

b) An alternative is a structured sentence resembling those used to record user stories and Architectural Decision Records (ADRs): 

<!-- For a definition of "risk treatment option", see page 44 of IEE Std. 7000, NOTE 2 -->

~~~
VBSR-m [name]:
To satisfy [EVR-n] and treat the risks related to it,
a H/M/L priority concern of [stakeholder name, individual role or group],
 * the SOI has to implement technical risk treatment option ... (and/or)
 * the organization developing and operating the SOI has to ... (and/or)
 * the following social construct(s) will have to be realized ...
~~~

Quality stories were proposed in the context of ["Architectural Refactoring for the Cloud"](http://rdcu.be/lFW6) (Springer Computing, 2016); the quality story template from that article may also be considered here.

Back to [Story Valuation page](/practices/ESE-StoryValuation.md#notations).

### Data Provenance 

```yaml
title: "ESE activity: Story Valuation"
author: Olaf Zimmermann (ZIO)
date: "07, 28, 2025 (Version 1.2)"
copyright: The author, 2023-2025 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```
