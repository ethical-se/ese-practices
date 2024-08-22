---
Scope: Larger unit (epic) or single feature/capability (story)
Phases: Product vision/upfront analysis and design; each sprint/iteration
Roles: Software engineer; product manager, user advocate, value lead
Input: Project goals and vision, business requirements, technical requirements; ConOps, (optional) existing Value Register
Output: New or updated Value Register, EVRs, (optional) VBSRs
---

Activity: *Story Valuation*
---------------------------
also known as Value-Enhanced User Story Elicitation, People-Society-Planet INVESTing 

<!-- TODO (v2) retrofit changes on ETHICOMP slides, process I7K comments on EVRs (?) -->

*Quick links:* (1) [Goal and Purpose](#goal-and-purpose) (2) [Notations](#notations) (3) [Techniques](#valuation-techniques) (4) [Usage](#usage) (5) [Application Hints](#hints-and-pitfalls-to-avoid) (6) [Other Practices](/practices/) (7) [ESE Home](/README.md)

### Context

According to Martin Fowler, software engineers are ["not just code monkeys"](https://www.youtube.com/watch?v=Z8aECe4lp44) but responsible and accountable for the software they build, its impact on users, society and the planet in particular. Ethical values guide responsible behavior; for instance, Annex G of [IEEE Std. 7000](https://ieeexplore.ieee.org/document/9967807) provides a collection of overarching core values. [^1] 

[^1]: Note that the value collection in the standard is informative, not normative; it does not aim to be complete.

In Agile software development, [user stories](https://socadk.github.io/design-practice-repository/artifact-templates/DPR-UserStory.html) serve as items in the [backlog](https://www.agilealliance.org/glossary/backlog/). When the Agile community members talk about value, they usually mean "business" value and end "user value"; story prioritization and progress tracking look at these two types of value (as well as realization effort). For instance, the 'V' in the INVEST [Definition of Ready](https://www.agilealliance.org/glossary/definition-of-ready/) has this very meaning.[^2]

Ethical Software Engineering (ESE), i.e., this project/repository, proposes to evaluate and assess epics and other stories w.r.t. their ethical values as well. This activity, described here, is called *Story Valuation*.

[^2]: *Excursion:* You may want to check the index of any book on Agile for the terms "ethics" and "values" to confirm this observation (or falsify it). Please open a PR or create an issue in this repository if you find ethical values in the Agile literature that ESE does not mention yet. 


### Goal and Purpose 

> *As a responsible software engineer, I want to craft working software that delivers value to users and other stakeholders while not harming any individuals, society and/or the planet. I want to identify goal conflicts so that adequate tradeoffs can be found.* 

Not doing any of the activities in ESE is possible, but may cause harm in the long run.[^3] 

Note that value requirements are a new, additional type of Non-Functional Requirements (NFRs) complementing and referring to functional (system) requirements (like other NFRs).

[^3]: Remember DieselGate?


### Instructions 
  
*Add individual, societal and environmental values to the business and user values in the "so that" part of epics, user stories or other types of product backlog items. Do so from the perspective of different stakeholder groups; compare and prioritize their value clusters and derive value requirements from them.*

Start this activity in [Product Vision](https://www.scrum.org/resources/what-product-vision) (or a Sprint 0 or an MVP development); return to it and resume valuation in each sprint/iteration as/if needed.

Apply one of the [techniques](#valuation-techniques) in ESE to do so and record your results in one of the proposed [notations](#notationso); alternatively, work with your own (or other recognized) techniques and notations; ESE is suggestive and not normative in this regard. 

#### Link to IEEE 7000

This activity corresponds to the following steps/phases in the process normed by IEEE Std. 7000: 

* "Ethical Values Elicitation and Prioritization Process" (Chapter/Clause 8)
* "Ethical Requirements Definition Process" (Chapter/Clause 9)

In IEEE Std. 7000 terms, story valuation populates the [Value Register](/ESE-Glossary.md#Value-Register) and yields [Ethical Value Requirements (EVRs)](/ESE-Glossary.md#EVR). Optionally (in ESE), the EVRs can be refined into [Value-Based System Requirements (VBSRs)](/ESE-Glossary.md#vbsr) as well. 

The following UML object instance diagram (aka Value Tree) illustrates the relationships (note that the EVRs, VBSRs, and DE are examples): 

![ESE/IEEE 7000 Value Tree](/images/ESE-ValueObjectTree.png)

<!-- TODO (v2) comment on L1 value vs. Value Demonstator (see ISD paper notes) -->

Note that the words [benefits](/ESE-Glossary.md#benefit) and [harms](/ESE-Glossary.md#harm) in the figure do not imply the usage, or sole usage, of any particular ethical theory.  

### Notation(s)

When following the above instructions to achieve the goal and purpose of Story Valuation, notations and/or text templates are required to record intermediate and final results; method techniques yielding such results are featured in [a later section](#valuation-techniques).

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

Collectively, the value epics, weightings, narratives comprise the Value Register for an SOI (or, picking up an agile term, the value backlog). See sections on techniques and examples for additional examples. 

***Disclaimer:*** These proposals have not been fully validated yet; please view them as drafts, serving as invitations to a continued method engineering discussion. [Examples](#examples) follow.

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


### Valuation Techniques 

The valuation techniques proposed in ESE are:

0. *Goals and Vision First*: [Question-Based Elicitation](#valuation-technique-0-question-based-value-elicitation-goals-and-risks-first) 
1. *User Requirements First*: [Story-Driven Value Jam](#valuation-technique-1-story-driven-value-jam-user-requirements-first)
2. *Individual Values First*: [Catalog-Guided Value Mapping](#valuation-technique-2-catalog-guided-value-identification-ethical-values-first)

Any combinations of these three techniques are eligible when following Agile methods. For instance, the [Product Vision](https://www.scrum.org/resources/what-product-vision) in Scrum may serve as a natural starting point for valuation activities, possibly using Question-Based Elicitation. Other techniques can be used and combined with the proposed three as well.

The valuation results are captured with the help of the above [notations](#notations). Please note that all three techniques focus on values at present; value requirements are only touched upon. For the time being, please refer to Clause 9 of IEEE Std. 7000 for more detailed EVR and VBSR elicitation and prioritization advice.

#### Valuation Technique 0: Question-Based Value Elicitation (Goals and Vision First)

To identify ethical values and elicit EVRs/VBSRs, you may want to ask the following questions when developing and hardening the product vision: 

1. How does the system (product, service) under construction make the world a better place? 
2. Even if there were no explicit, external stakeholder goals and business drivers, why is it still a good idea to develop the system?  Which positive ethical values does it promote?
3. Which positive ethical values are degraded by any realizations of the envisioned functionality?  Which negative values are promoted? What are the related elements of risk, those with high probability and huge impact in particular?
4. How do positive and negative values, as well as [benefits](/ESE-Glossary.md#benefit) and [harms](/ESE-Glossary.md#harm), relate to each other? What is their relative and/or absolute weight?
5. Which resources will the system consume, and can this consumption be justified by the business/user and ethical values that it delivers? 

The questions should be answered in close cooperation with end users and business representatives as well as other key stakeholders; epics and stories are invitations for conversations.

![Value Elicitation Questions](/images/ESE-ValueElicitationQuestions.png)

With these questions answered (from the perspective of each stakeholder group) and prioritized, INVEST becomes INVEST+ (see [Definition of Ready](ESE-DefinitionOfReady.md)). The answers to the questions can be noted as Value Epics, Value Weightings and/or Value Narratives (see section on notations). Some answers actually populate (or enhance) the IEEE Std. 7000 [ConOps](/ESE-Glossary.md#conops); they can be seen as part of the [Context Exploration Process (CEP)](/ESE-Glossary.md#cep). <!-- Clause 7 in standard; see our [Glossary](/ESE-Glossary.md) for definitions from the standard. -->

*Note:* When dealing with Systems of Systems (SoS), the questions can be asked for each involved system as well as the SoS itself. See Annex E of IEEE Std. 7000 for more information on ethic control considerations in SoS.


#### Valuation Technique 1: Story-Driven Value Jam (User Requirements First)

An alternative to starting from open questions (as in technique 0) or Annex G of IEEE Std. 7000 (technique 2) is to look at epics or a set of stories in the backlog and ask questions about their content parts:[^4]

[^4]: This works for [use cases](https://socadk.github.io/design-practice-repository/artifact-templates/DPR-UseCase.html) too.

* What are the individual and collective values of the persona/role in the "As a" part of the story (aka stakeholder groups)? 
  * Which responsibilities do their user interfaces have that may promote or degrade ethical values (both positive and negative ones)? 
* Which ethical values are affected when executing the program code realizes the "I want to" part of the story? 
* What is the desired and, presumably, actual impact (good and bad) of the "so that" part of the story on individuals, society, and planet?

![From Story to Value Clusters](/images/ESE-StoryToValueCluster.png)

*Optional:* The "I want to" featured might also suggest questions about data display, processing, storage and exchange (do any of these design elements have ethical relevance?):[^5] 

* Which values are affected positively or negatively when end user input is received and validated? When computation and query output is displayed?
* How does the data processing (application/business/domain logic) do w.r.t values?  
* How do data access components and data storage (persistence mechanisms) behave w.r.t. values? 
* What is the ethical risk of APIs and other transport channels, as well as shared services such as loggers?

[^5]: Some of these questions look ahead somewhat and concern design issues (on a rather abstract level).

Having answered the questions once, next steps may include to: 

* Ask similar questions from the perspective of key stakeholder groups not represented as personas/roles in the epic or story that is analyzed. For instance, investigate the values of service providers involved in story fulfillment. 
* Prioritize and record the answers to these questions, for instance in a value tree or a value-enhanced use case diagram. 

Again, the answers to the questions can be noted as Value Epics, Value Weightings and/or Value Narratives (but also other [Notations](#notations)). These artifacts then populate the Value Register for the [System of Interest (SOI)](/ESE-Glossary.md#soi). The technique may also yield a set of [EVRs](/ESE-Glossary.md#evr) and [VBSRs](/ESE-Glossary.md#vbsr), which can be stated as value-enhanced user stories or value QAS.


#### Valuation Technique 2: Catalog-Guided Value Identification (Ethical Values First)

Annex G in [IEEE Std. 7000](https://ieeexplore.ieee.org/document/9536679), which is suggestive, not normative, provides 12 examples of core/overarching values in Table G.1.[^6] Next-level values, both related and opposing, are also suggested in Annex G (pages 69-70).
A value-first approach might start from these rather abstract and generic values, but also other ones identified by the team; the standard encourages adopters to add other values as required or desired in a particular context and culture. 

![Valuation Steps](/images/ESE-ValuationTechniqueValuesFirst.png)

[^6]: For example, Accountability is not listed as a top 12 overarching/core value in Annex G, but is mentioned several times in IEEE Std. 7000.

<!-- 

| Ethical value applicable to system design | Related value | Opposing value |
|-|-|-|
| | | |

"Autonomy Moral agency, dignity, independence, freedom, liberty, mobility, self-direction, power, self-actualization, ownership; Accountability, responsibility, responsiveness, reciprocity, paternalism, slavery
Care Accountability to shareholders, investors, suppliers, and other stakeholders; understanding; compassion; love; empathy; protection of the vulnerable; affection; support; friendliness; beneficence; benevolence; generosity; gentleness; helpfulness; kindness; comfort; quality of life; paternalism; Torture, maleficence, persecution, machine capability, logic, objectivity
Control Human responsibility, governance, usability, portability, logic, sense of accomplishment, moderation; Trust, accountability to stakeholders; imagination, reminding, obedience
Fairness Responsible position on conflicts of interest, tolerance, justice, balance, equality (legal, gender, minority); Bias, suspicion, discrimination, arbitrariness
Inclusiveness Participation, partnership, solidarity, interdependence, compatibility, accessibility, diversity; Control, bias, detachment
Innovation Modifiability, adventure, novelty, excitement, playfulness, diversity, development, learning, curiosity, creativity; Tradition, distraction
Perfection Integrity, truth, honesty, achievement, transcendence, universalism, wisdom; Competence, feasibility, over-capacity,
Privacy Respect for confidentiality, intimacy, anonymity; Transparency, inclusiveness, alerting
Respect Politeness, courtesy, respect for environment and natural habitat, respect for information and confidentiality, respect for norms, reputation; Self-esteem, maleficence
Sustainability Respect for environment and natural habitat, efficiency, maintainability, operability, supportability, reliability, durability, resilience, forgiveness, robustness, redundancy, reusability, re-configurability, simplicity, economy, renewability; Cost (extravagance), wastefulness, poverty, consumption
Transparency Openness, cleanliness, explicability, explainabililty, access to data. auditability; Privacy, bribery, corruption 
Trust Predictability, dependability, veracity; Control

NOTE: Opposing values can be positive or negative."
-->

The following steps can be followed when applying the technique: 

1. *Pick 2-3 core values from the table.* Use the information in the columns "Related value" and "Opposing value" columns in Table G.1 to make them more complete, concrete, and tangible.
2. *Explain the relevance of each core value in the given project/product context by way of example and/or refinement.* You might want to tell a story and/or point out the positive and negative consequences of this value in the form of a narrative (see column in table above). This information may come from the Value Register of the project/product development effort when IEEE Std. 7000 is followed (if no Value Register exists yet, it is a good time to create one now).  
3. *Prioritize the value(s), either absolutely or relatively.* For instance, you may want to use a writing style similar to that in the Agile Manifesto ("We value mm over nn").

Repeat these steps for each stakeholder group. Keep an eye on effort, focus on and begin with high-priority, high-impact values. 

You may want to record the results of Steps 1 to 3 in table form or another [notation](#notations):

| Overarching Value (Core) | Related Values (Themes) | Priority | Potential Conflicts (Opposing Values) | Story/Narrative/Demonstrator/Example |
|-|-|-|-|-|
| Autonomy | | H/M/L |  |  |
| *additional value n* | | H/M/L | | |
| ... | | H/M/L | | |

The filled-out table becomes the Value Register; the technique may also yield EVRs and VBSRs when refining the Story/Narrative/Demonstrator/Example entries in the table by asking "How are we going to realize/achieve ...?" questions during production vision work, requirements analysis and (early) design.



### Examples 

#### Example 1: Same Day Delivery in an Online Shop 

Take this high-level user story (aka epic):

> *As an online shopper, I would like to receive ordered goods on the same day so that I can respond to emergency situations and use my time efficiently.* 

The following example may result from an application of Valuation Technique 1, [User Requirements First](#valuation-technique-1-story-driven-value-jam-user-requirements-first). Its (incomplete, initial) story-based valuation may yield the following *Value Case Diagram*: 

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

<!-- user story taken from PfAD book, Chapter 2; TODO (v2) could also add NFRs from there -->

> *As a customer of Lakeside Mutual, I want to update my contact information myself online so that the data is current. I do not want to have to call an agent for that, which may involve long waiting times.*

On the first sprint/iteration of a related agile development project, the [Value Lead](/roles/ESE-ValueLead.md) asks the Senior [Product Manager](/roles/ESE-ProductManager.md), also serving as [User Advocate](/roles/ESE-UserAdvocate.md), and a System Expert to join her for a Story Valuation about the Customer Profile and Offer Management stories. She also takes the role of Moderator (see IEEE Std. 7000 for explanations of the System Expert and Moderator [roles](/roles/)).

The participants decide to start with Valuation Technique 2, [Values First](#valuation-technique-2-catalog-guided-value-identification-ethical-values-first), and blend in elements from the other two techniques. They come up with the following table:

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

This example features technique 0, [Goals and Vision First](#valuation-technique-0-question-based-value-elicitation-goals-and-vision-first) and the alternative notations not yet exemplified.

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

<!-- TODO (v2) find more examples of "social constructs" and clarify origin of term. <https://en.wikipedia.org/wiki/Social_construct>-->

~~~
VBSR-1 CIA-Security:
To satisfy the desire for data privacy and treat risks related to this core value,
a H(igh) priority concern of conference participants,
 * the SOI has to implement HTTPS as technical treatment option and
 * the organization developing and operating the conference registration system has to restrict access to participant data and
 * understandable terms and conditions will have to be realized (as a social construct).
~~~

***Note:*** *This version of ESE does not provide any sample output of business-as-usual software engineering activities such as architecture design and implementation. That said, sample [Architectural Decision Records (ADRs)](https://medium.com/olzzio/how-to-review-architectural-decision-records-adrs-and-how-not-to-2707652db196) are featured in the example of an Ethical Review. See [Future Work](/ESE-FutureWork.md) for related method engineering ideas and plans.*

<!-- TODO (v2) elaborate: What's next? Consequences (good and bad)? More discussions with stakeholders, less business growth but "gutes Gewissen". Some more work too. But less risk. See JEDi user stories and VDAD steps 4 to 7. -->

The section on [notations](#notations) proposes the templates for this step that are featured in the examples.

### Usage

The Story Valuation activity in ESE complements and extends the original meaning of the V in INVEST to include ethical values, whatever these may be in a given project context. 

W.r.t. analysis and planning activities, Story Valuation output is asked for in the value-enhanced [Definition of Ready](ESE-DefinitionOfReady.md). It is an essential input to risk management.
The [Definition of Done](ESE-DefinitionOfDone.md) asks whether the Story Valuation output has been respected in design, implementation and Acceptance Testing.
EVRs and VBSRs drive design and implementation activities; they justify [architectural decisions](https://en.wikipedia.org/wiki/Architectural_decision). Transitioning to general software engineering and [design practices](https://socadk.github.io/design-practice-repository/), components in architecture models can be traced back to them; [Domain-Driven Design (DDD)](https://ozimmer.ch/modeling/2022/11/23/ContextMapperInsights.html) can make the values and resulting requirements visible and explicit in its models as well. 


### Hints and Pitfalls to Avoid

Note that values can be positive and negative (see for instance coverage of "Value axioms" in Annex B of IEEE Std. 7000). Hence, it is important to:
 
* *Identify and document goal conflicts.* Conflicts will arise, for instance between groups of stakeholders and their concerns (e.g., those of customers and sponsors/owners of a software product and those of the product development team), between business requirements and ethics, and between technology choices and ethics. If a severe taboo conflict arises and cannot be resolved, terminate the sprint and reconsider whether the epic or story that caused the conflict should actually be implemented. Decide to go [separate ways](https://ddd-practitioners.com/home/glossary/bounded-context/bounded-context-relationship/separate-ways/) if necessary. 
* *Be inclusive and communicate.* Faithful to Agile values, developers and other software engineering roles should not guess or make up any user requirements (including value expectations) but learn about them in conversations. Stakeholders are different, and so are their values and value priorities. All stakeholders and their value concerns should be listened to, not just the end user personas appearing in the "As a" role part of stories.
* *Stay focussed.* 100s of values might be affected, but only the most important ones (see Table B.1 on page 55 in IEEE Std. 7000 and/or "Material Ethics of Value" by Eugene Kelly to find those) can be investigated in depth, realistically.
* *Manage and trace.* It is important to keep track of the IEEE Std. 7000 artifacts (ConOps, Value Register, EVRs, VBSRs) as they are updated during design and implementation. 

Here are four more items of advice: 

*  *Have an eye on effort vs. benefit.* If your stories are rather fine-grained in similar w.r.t. values, you might want to perform the Story Valuation on the epic level, starting when establuishing the Product Vision.
* *Adopt the practice according to project/product context.* For instance, you might want to combine the proposed goals-first, requirements-first, and values-first valuation techniques in a meet-in-the-center approach. Business domains, application genres and domain patterns (a term from the book ["Domain-Driven Transformation"](https://www.wps.de/aktuelles/domain-driven-transformation) by Carola Lilienthal and Henning Schwentner) bring different values and value prioritizations with them naturally. 
* *Welcome change.* Story Valuation might lead to new stories, to changes in existing stories (which in turn might no longer satisfy INVEST and have to be split), to new engineering/quality requirements for existing stories. [Software crafts(wo)manship](https://en.wikipedia.org/wiki/Software_craftsmanship) comes to mind, stating that steadily adding value is as important as welcoming change.
* *Start early.* See [FAQ](/ESE-FAQ.md) on when to perform the IEEE 7000 Std. processes. Sprint zeros, proof-of-concepts, architectural spikes or MVP developments provide opportunities to establish value-based design thinking early (these Agile concepts have been captured as [patterns](https://socadk.github.io/patterns/reading-lists/agile-architecture.html)). 

Final advice is: 

* Note the difference between values (positive and negative) and consequences of acting along those values (also known as benefits and harms). Values cannot be taken for granted and universally agreed upon but have to be established (also see [FAQs](/ESE-FAQ.md), those on IEEE Std. 7000 in particular).
* Use *checklists* such as ["Questions to Ask when Migrating to the Cloud"](https://medium.com/olzzio/questions-to-ask-when-migrating-to-the-cloud-dcbf7c5febdf) to learn about the context and usage of existing systems.
* Let the value-assessed stories (elicited in this activity) serve as input to value-based design decision-making. Capture the *rationale* for the decisions and include EVRs and VBSRs in the resulting [decision records](https://medium.com/olzzio/from-architectural-decisions-to-design-decisions-f05f6d57032b).
* Validate and verify the *realization* of value-assessed stories in [Ethics Reviews](ESE-EthicalReview.md).

<!-- TODO (v2) include a Stakeholder Type mind map and give advice, map to roles in standard: types/roles/personas, e.g. occasional and regular end user, differing values and usability needs -->

### Related Content

* The Product Backlog contains the stories to be valuated.
* Sprint Planning picks stories from the backlog. Story Valuation is performed for each story selected for a sprint during Story Planning (but not part of it), or for a set of related stories such as those for an epic. It may happen during Production Vison work, in a Sprint 0 or in MVP development too (see related question in [FAQs](/ESE-FAQ.md)).
* The [Definition of Ready](ESE-DefinitionOfReady.md) checks whether Story Valuation has been performed adequately; the [Definition of Done](ESE-DefinitionOfDone.md) asks whether the Story Valuation output has been respected in design, implementation and Acceptance Testing.
* The [Ethical Review](ESE-EthicalReview.md) meeting and report compare Story Valuation output and design/implementation.  
* A [Value Retrospective](ESE-ValueRetrospective.md) reflects whether and how Story Valuation (and other ESE practices) can be improved.

ESE does not contain any design practices at present; the [Design Practice Repository and Reference (DPR)](https://socadk.github.io/design-practice-repository/) collects essential ones that continue to be relevant in ESE. 


### More Information 

Ethical values <!-- and ways to handle them --> are covered in the following publication and online resources (selection): 

* The article ["Human Values as the Basis for Sustainable Information System Design"](https://research.wu.ac.at/ws/portalfiles/portal/19837176/Human+Values+as+the+Basis+for+Stustainable+Information+Systems+Design+%28Pre-print%29.pdf) has many more examples of values.
* IEEE Std. 7000 and literature on "Material Value Ethics" may help with prioritization: 
  * For instance, advice is given in Clause 8.3, Step d) on page 41; seven types of ethical considerations and three external sources are listed. Table B.1 in Annex B of IEEE Std. 7000 summarizes five principles for value ranking and provides examples; Table D.1 in Annex D lists legal, societal, and environmental feasibility study guidelines (pages 62 to 64). 
  * And ["Value-Sensitive Design"](https://mitpress.mit.edu/9780262039536/value-sensitive-design/) compiles 13 human values in Table 2.1 on page 28; Table 3.1 on pages 61 to 64 summarizes 17 value-sensitive design methods.
* A 2019 conference presentation by Jennifer Riggins called ["How (and Why) to Factor Tech Ethics into Your Sprint"](https://www.infoq.com/presentations/tech-ethics-sprint/) and her article ["Tech Ethics New Year’s Resolution: Don’t Build Software You Will Regret"](https://thenewstack.io/tech-ethics-new-years-resolution-dont-build-software-you-will-regret/) ask valuation questions, effectively forestalling/antedating our three valuation techniques, for instance "What is the worst possible use case for this code?" Other questions concern connectivity and data transfer as well as data storage and lifetime.
* Annex B of IEEE Std. 7000 covers value concepts, starting from philosophical foundations in B1; B2 presents an example and B.4 covers value ranking. Annex C is about ethical theories applied to ethical value elicitation, for instance, utilitarian ethics, virtue ethics, and duty ethics.
* The [Proctive Consider, Analyze, Review, Evaluate (CARE)](https://ethics.acm.org/wp-content/uploads/2021/03/Proactive-CARE-for-Computing-Professionals.pdf) framework and [Software Development Impact Statements (SoDIS)](https://doi.org/10.17705/1CAIS.01540) as well as the [Consequence Scanning](https://doteveryone.org.uk/project/consequence-scanning/) practice also propose an active, "push" approach to knowledge sharing (just like ESE). Some of the questions raised in these publications and practices overlap with the ones in ESE; others are complementary.  
<!-- TODO (v2) list JEDi here when public -->
  
More information about the INVEST principles/criteria is available in many places: 

* [Wikipedia page](https://en.wikipedia.org/wiki/INVEST_(mnemonic)) for INVEST
* ["New to agile? INVEST in good user stories"](https://agileforall.com/new-to-agile-invest-in-good-user-stories/) on Agile for All website
* ["10 Tips for Product Owners on the Product Vision"](https://www.scrum.org/resources/blog/10-tips-product-owners-product-vision) in Scrum

Other related practices and concepts include: 

* Project Charter, see <https://www.agilealliance.org/glossary/project-chartering/> 
* DPR has a [User Story](https://socadk.github.io/design-practice-repository/artifact-templates/DPR-UserStory.html) artifact. There is an overview article on DPR on [Medium](https://medium.com/olzzio/design-practice-repository-and-reference-gitpages-and-ebook-enhanced-f43c107f2567).
* The role-feature-benefit template for user stories is explained [here](https://www.agilealliance.org/glossary/user-story-template/).
* Card, Conversation, Confirmation (3Cs) in [Agile Glossary](https://www.agilealliance.org/glossary/three-cs).

The [Agile Glossary](https://www.agilealliance.org/agile101/agile-glossary/) is a good reference for Agile practices.


### Data Provenance 

```yaml
title: "ESE activity: Story Valuation"
author: Olaf Zimmermann (ZIO)
date: "11, 20, 2023 (Source: Project ESE)"
copyright: The author, 2023 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```
