---
Scope: Larger unit (epic) or single feature/capability (story)
Phases: Product vision/upfront analysis and design; each sprint/iteration
Roles: Software engineer; product manager, user advocate, value lead
Input: Project goals and vision, business requirements, technical requirements; ConOps, (optional) existing Value Register
Output: New or updated Value Register, EVRs, (optional) VBSRs
---

Examples for Activity: [*Story Valuation*](/practices/ESE-StoryValuation.md)
---------------------------

### Examples 

#### Example 1: Same Day Delivery in an Online Shop 

Take this high-level user story (aka epic):

> *As an online shopper, I would like to receive ordered goods on the same day so that I can respond to emergency situations and use my time efficiently.* 

The following example may result from an application of Valuation Technique 1, [User Requirements First](/practices/ESE-StoryValuation.md#valuation-technique-1-story-driven-value-jam-user-requirements-first). Its (incomplete, initial) story-based valuation may yield the following *Value Case Diagram*: 

![](/images/ESE-ValueCaseDiagramExample.png)

The diagram displays the Story Valuation result on value level. A collection of such Value Case Diagrams forms a lightweight Value Register (no explicit EVRs and VBSRs included in this example).  

A related Value Narrative might be:

~~~
When the online shopping software executes the same say delivery epic (incl. split user stories that meet the INVEST criteria),
stakeholders expect it to promote freedom and quality of life,
possibly degrading or prohibiting work-life balance of suppliers and shopper privacy
by exposing the following externally observable behavior:

Given: Shop is operational and suited suppliers and logistics firms are available. 
When: Same day delivery is promised during order acceptance and confirmation. 
Then: Order arrives at shipment address until 11:59pm on the same say.   
~~~


#### Example 2: Insurance Scenario and System of Interest (SOI) 

Let's use the Customer Self Service of [Lakeside Mutual](https://github.com/Microservice-API-Patterns/LakesideMutual) as an exemplary SOI. Let us assume that its ConOps has already been analyzed and documented. 

> *As a customer of Lakeside Mutual, I want to update my contact information myself online so that the data is current. I do not want to have to call an agent for that, which may involve long waiting times.*

On the first sprint/iteration of a related agile development project, the [Value Lead](/roles/ESE-ValueLead.md) asks the Senior [Product Manager](/roles/ESE-ProductManager.md), also serving as [User Advocate](/roles/ESE-UserAdvocate.md), and a System Expert to join her for a Story Valuation about the Customer Profile and Offer Management stories. She also takes the role of Moderator (see IEEE Std. 7000 for explanations of the System Expert and Moderator [roles](/roles/)).

The participants decide to start with Valuation Technique 2, [Values First](/practices/ESE-StoryValuation.md#valuation-technique-2-catalog-guided-value-identification-ethical-values-first), and blend in elements from the other two techniques. They come up with the following table:

| Overarching Value (Core) | Level 1 Values (Themes) | Priority | Potential Conflicts (Opposing Values) | Narrative/Demonstrator |
|-|-|-|-|-|
| Autonomy | Freedom | M | Accountability, auditability NFR | Profile management, archiving work with [Sensitive Personal Information (SPI)](https://www.linkedin.com/pulse/gdpr-approaches-protecting-personally-identifiable-wittkop-cissp) |
| Fairness | Justice, equality | H | Bias | Offer preparation: insurance rates, risk uplifts |
| Privacy | Confidentiality | H | Transparency | SPI transport, statistics (analytics) |

They record the following prioritization and scoping decisions of core values, accompanied by value demonstrators: 

1. *Autonomy:* Customers should at any time be able to fully delete all information stored about them without having to provide any reason for that. The effect of the deletion is immediate. *Value rationale:* The team values freedom more than accountability and auditability.
2. *Fairness:* When an offer is made, the premium is based solely on demographic information that the customers opted in to provide and use. There is no personal judgment of any human being or any machine intelligence drawing from other sources involved. *Value rationale:* Concerning the overarching value of fairness, justice is strived for and bias to be avoided. 
3. *Privacy:* Although regulators and other lines of business have a legitimate interest in the data collected, it remains on-premises and within the application boundary of the Lakeside Mutual services (backends). *Value rationale:* The team values data confidentiality over (certain facets of) transparency.

One of the EVRs derived from these value demonstrators could be:

~~~
As a prospective customer of Lakeside Mutual,
I want to manage my data profile autonomously 
so that I am offered a valid and fairinsurance rate 
  while my data remains private (data privacy is promoted),
  accepting that accountability and auditability cannot be fully achieved.
~~~

A Value Quality Scenario for this example might be:

|  | Profile Autonomy and Transparency Scenario |
|-|-|
| *Stimulus* | Read and write requests to User Profile Management (Story-form EVR stated previously) |
| *Concern Of (Source)* | Prospective and actual customers |
| *Observable When* | Profile is retrieved and displayed, offers are made (normal system operations, edge and error cases too) |
| *Materializing In* | Customer database in Policy Management and Customer Core services of Lakeside Mutual systems, the [SOIs](/ESE-Glossary.md/#soi) |
| *Value Requirement/Response* | There is one and only one API for the Customer profile, which is only accessed from the Customer Self Service and the Policy Management backends; data used for rate calculation is transparent/explained to customer |
| *Value Requirement/Response Measure* | 0 data breaches, no use of data that is not specified |

In this example, the Story Valuation output yields a new Value Register entry (value cluster), a new EVR, and a new VBSR.

The analysis and design work in the first and following sprints/iterations (that pull other stories, or work with those resulting from [splitting](https://socadk.github.io/design-practice-repository/activities/DPR-StorySplitting.html) the rather broad one on Customer Self Service). Among other agile practices, the following design practices are used:  

* [SMART Non-Functional Requirement (NFR) Elicitation](https://socadk.github.io/design-practice-repository/activities/DPR-SMART-NFR-Elicitation.html), possibly yielding "Agile Quality Scenarios", see this [pattern collection](https://socadk.github.io/patterns/reading-lists/agile-architecture.html).
* [Architectural Decision Capturing](https://socadk.github.io/design-practice-repository/activities/DPR-ArchitecturalDecisionCapturing.html), referring to SMART NFRs including EVRs and/or VBSRs in the decision justifications (design rationale).
* [Architecture Modeling](https://socadk.github.io/design-practice-repository/activities/DPR-ArchitectureModeling.html), featuring design elements that are introduced to satisfy EVRs and VBSRs.


#### Example 3: Conference Management 

This example features technique 0, [Goals and Vision First](/practices/ESE-StoryValuation.md#valuation-technique-0-question-based-value-elicitation-goals-and-vision-first) and the alternative notations not yet exemplified.

<!-- TODO (v2) use different sample values from Annex G (?) -->
~~~
As a conference participant,
I value data privacy,
as demonstrated in: 
- a realization of confidentiality of sensitive personal information such as my passport number 
- a reduction of efficiency of operations for conference mansagement staff.
This value cluster has high priority for me. 
~~~

~~~
In the context of the conference registration system,
conference participants value data privacy more than efficiency from a registration management staff point of view,
expecting benefits such as confidentiality of sensitive personal information
running the risk of harms such as higher conference fees and a slower registration process.  
~~~

<!-- TODO (v2) find more examples of "social constructs" and clarify origin of term. <https://en.wikipedia.org/wiki/Social_construct> B. Bohr, IEEE Software paper? -->

~~~
VBSR-1 CIA-Security:
To satisfy the desire for data privacy and treat risks related to this core value,
a H(igh) priority concern of conference participants,
 * the SOI has to implement HTTPS as technical treatment option and
 * the organization developing and operating the conference registration system has to restrict access to participant data and
 * understandable terms and conditions will have to be realized (as a social construct).
~~~

***Note:*** *This version of ESE does not provide any sample output of business-as-usual software engineering activities such as architecture design and implementation. That said, sample [Architectural Decision Records (ADRs)](https://medium.com/olzzio/how-to-review-architectural-decision-records-adrs-and-how-not-to-2707652db196) are featured in the example of an Ethical Review. See [Future Work](/ESE-FutureWork.md) for related method engineering ideas and plans.*

<!-- TODO (v2) elaborate: What's next? Consequences (good and bad)? More discussions with stakeholders, less business growth but "gutes Gewissen". Some more work too. But less risk. See VDAD user stories and VDAD steps 4 to 7. -->

The [notations](/practices/ESE-StoryValuation-Notation.md) page proposes the templates for this step that are featured in the examples.

Back to [Story Valuation page](/practices/ESE-StoryValuation.md#examples).

### Data Provenance 

```yaml
title: "ESE activity: Story Valuation"
author: Olaf Zimmermann (ZIO)
date: "07, 28, 2025 (Version 1.2)"
copyright: The author, 2023-2025 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```
