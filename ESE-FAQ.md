## Frequently Asked Questions about Ethical Software Engineering (ESE)

### Perception and Adoption of [IEEE Std. 7000](https://standards.ieee.org/ieee/24748-7000/11098/) 

* How does ESE use and integrate concepts from the standard, for instance its Value Register? 
  * *Answer:* ESE provides mapping tables for the processes in the standard, see [background information](ESE-BackgroundInformation.md#from-ieee-std-7000-processes-to-agile-practices). It does not enforce any particular template or notation for the artifacts and concepts (also including EVRs and VBSRs), but suggests them, as well techniques to create them with a little extra effort as possible. See for instance the three techniques for Story Valuation. That said, there is a folder with work-in-progress [Markdown templates](/templates) for the standards artifacts (subject to change at any time).  
  
* When should [ConOps](/ESE-Glossary.md#conops), [Value Register](/ESE-Glossary.md#value-register), [EVRs](/ESE-Glossary.md#evr) be written up? On a project or before?   
  * *Answer:* A Sprint/Iteration 0 can be performed to carve out [epics](https://www.agilealliance.org/glossary/epic/) and yield system context diagrams. Early value-related artifacts (ConOps, Value Register with initial set of EVRs) can then accompany these. Each development sprint/iteration can then derive VBSRs from the EVRs and update the existing artifacts as more and more information becomes available. See "Misc" section below for acronym resolution!

* What is the difference between EVRs and VBSRs? 
  * *Answer:* See [glossary](/ESE-Glossary.md) entries for definitions. VBSRs refine EVRs; see Annex B and full-body scanner example in B.2 for sample EVR(s) and VBSR(s). Note that in ESE, VBSRs optional; ADs can be made based on EVRs that may take story form in ESE.

* Are all values positive?
  * *Answer:* No, that is a misperception. Material ethics provide elaborate definitions and discussion. From IEEE 7000, Annex B.3: "Positive and negative values interrelate in the following way (Axioms of Material Value Ethics): <!-- Section 5.6 on page 30 lists and discusses three ethical theories used to elicit values. -->
    a) The existence of a positive value is itself a positive value. 
    b) The non-existence of a positive value is itself a negative value. 
    c) The existence of a negative value is itself a negative value. 
    d) The non-existence of a negative value is itself a positive value."   

* Does IEEE Std. 7000 recommend or depend on any particular "school" of ethics?
  * *Answer:* It does not. See Section "5.6 Ethical theories used to elicit values". Adopters are encouraged to add what they want and need.
   
* The four processes in the standard come across as rather heavyweight. Is that true? 
  * *Answer:* It depends.[^1] Methods can and should be tailored to a particular context and need; this is what ESE is all about. See our guiding principles and method adoption rules for [DPR](https://medium.com/@docsoc/design-practice-repository-dpr-ed5e9d0e91cd).

* The overall process flow left a "waterfall!" impression on me. Any thoughts?  
  * *Answer:* A text document has to be ordered sequentially. You can spend as much or little time on each step and activity as you want (and are used to), and it is perfectly fine to go back often. See our [practices](/practices). 
    
* How can the top-level management support that the standard calls for be obtained in agile settings? Aren't teams supposed to operate autonomously?
  * *Answer:* Safe and other approaches to scaling agile can have a role to play. The same management that backed the introduction of agile practices is an ideal choice. 

[^1]: It depends of course... see [here](https://www.consultantsmind.com/2013/05/13/the-best-short-answer-to-give-clients-it-depends/) and [here](https://www.linkedin.com/pulse/depends-demystifying-common-consultant-answer-jacob-chandler) for explanations and some criteria.


### Agile Values and Principles

* Does usage of IEEE Std. 7000 introduce the risk of harming project velocity?
  * *Answer:* Our motivation in this work is to prevent this. Some slow down might actually be beneficial as value elicitation and conflict resolution do take time and require rigor and effort. The more critical a system is (think about safety-critical systems), the more effort and time for careful, responsible analysis and design work is in order.

* How do the Agile values in the manifesto and those in XP etc. fit in?
  * *Answer:* While related, not all of the agile values directly correspond to ethical values such as transparency, sustainability, privacy, fairness, and accountability. The following table maps the four values of the Agile Manifesto to selected, exemplary core values from Table G.1 in IEEE Std. 7000:

| Agile Value ([source](https://agilemanifesto.org/))| IEEE 7000 Core Value (Examples) | Comments |
|-|-|-|
| "Individuals and interactions over processes and tools" | Autonomy, Respect, Trust | Tailoring required |
| "Working software over comprehensive documentation" | Care, Innovation, Sustainability| Light templates, aligned with existing ones |
| "Customer collaboration over contract negotiation" | Control, Inclusiveness, Trust | Roles: User Advocate, Moderator, Value Lead |
| "Responding to change over following a plan" | Fairness, Perfection, Transparency | Frequent updates required to learn adaptively and achieve goals eventually |

The absence of Privacy is worth noting. Other mappings are possible as well. As an exercise to get familiar with the ethical values, try filling out the table yourself.

* How do the twelve Agile principles (for manifesto) fit in?
  * *Answer:* See the following table:
  
The 12 principles, also quoted from the Agile Manifesto, map to IEEE Std. 7000 (Annex G) nicely as well. Example mappings include (as noted, others can be found):

| Principle ([source](https://agilemanifesto.org/principles.html)) | IEEE 7000 Core Value, Related Value | Comments |
|-|-|-|
| 1. "Our highest priority is to satisfy the customer through early and continuous delivery of valuable software." | Care: accountability to stakeholders | Other mappings possible |
| 2. "Welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage." | Innovation: modifiability, adventure | Other mappings possible |
| 3. "Deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale." | Control: sense of accomplishment, governance | Other mappings possible |
| 4. "Business people and developers must work together daily throughout the project." | Inclusiveness: participation, partnership | Other mappings possible |
| 5. "Build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done." | Trust: dependability | Other mappings possible |
| 6. "The most efficient and effective method of conveying information to and within a development team is face-to-face conversation."| Respect: politeness, courtesy | Other mappings possible (?) |
| 7. "Working software is the primary measure of progress." | Transparency: explicability, openness | Other mappings possible (?) |
| 8. "Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely." | Respect: politeness, courtesy | Other mappings possible |
| 9. "Continuous attention to technical excellence and good design enhances agility." | Perfection: achievement | Other mappings possible (?) |
| 10. "Simplicity - the art of maximizing the amount of work not done - is essential." | Sustainability: simplicity | Other mappings possible |
| 11. "The best architectures, requirements, and designs emerge from self-organizing teams." | Autonomy: self-direction | Other mappings possible |
| 12. "At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly." | Fairness: balance, tolerance | Respect and trust required |

Note that Privacy is absent from the examples; values such as Respect and Trust relate to several other Agile principles.

### ESE and other methods/assets

* How do IEEE Std. 7000 and ESE relate to the [ACM Code of Ethics and Professional Conduct](https://www.acm.org/code-of-ethics) and similar codes (including those on ethical artificial intelligence)?
  * *Answer:* IEEE Std. 7000 specifies processes, applicable for organisations, teams, projects; ESE adds practices to integrate the standards concepts into agile development. Complementarily, codes such as the ACM one focus on individuals and their behavior. The standard, the codes, and ESE share common goals such as raising awareness for the existence and importance of ethical values and moral obligations in the context of systems and software engineering.

* How does ESE relate to the [Proactive CARE framework](https://ethics.acm.org/wp-content/uploads/2021/03/Proactive-CARE-for-Computing-Professionals.pdf), available on the ACM ethics website?
  * *Answer:* See the following table: 

| Proactive CARE (Gotterbarn et al) | IEEE Std. 7000, ESE |
|-|-|
| "Consider who might be affected and how"| ConOps work, case for ethics (IEEE Std. 7000), Story Valuation techniques (ESE) | 
| "Analyze the situation’s details"| Ethical Value Requirement (EVR) elicitation, follow-on design work, reviews | 
| "Review other obligations and limitations"| Work on ConOps, EVRs | 
| "Evaluate the best course of action"| Design decision making | 

* Can ESE be combined with other methods and description standards? 
  * *Answer:* Yes. For instance, in [arc42](https://www.arc42.de/) descriptions, the ESE output could go to a new section ("arc42+") or to existing ones: 

1. Introduction and goals could talk about core values.
2. Constraints could add first EVRs.
3. Constraints Context and scope is the right place for ConOps information.
4. The Solution Strategy could pick up and extend the core values and add more EVRs.
5. Sections 5 to 9 then cover design, as usual.
6. Section 10 might have the full set of EVRs and also VBSRs.
7. Section 11 might pick up the risk-oriented approach of IEEE Std. 7000.
8. The glossary refers to the ESE glossary and also explains the solution-specific values.


### Misc

* What do all the acronyms mean (EVR, SOI, VBSR, ...)? 
  * *Answer:* See the [Glossary](/ESE-Glossary.md#overview).

* What is available in ESE (this repository)? 
  * *Answer:* ESE describes two new [practices](/practices/), Story Valuation and Ethics Review, and extends three existing ones, Definition of Ready, Definition of Done, and Retrospective. It also features [roles](/roles/) from IEEE Std. 7000. 

* How is ESE organized? 
  * *Answer:* See the following figure:
![ESE Building Blocks](/images/ESE-BuildingBlocks.png)

* What does the Story Valuation practice contain? 
  * *Answer:* See the following figure:
  
![ESE Story Valuation Structure](/images/ESE-SVStructure.png)
  
* Is there a "minimum viable adoption" of ESE and/or a lightweight way of applying IEEE Std. 7000? 
  * *Answer:* Story Valuation and Ethics Review are the two essential ESE practices. You can view existing practices and notations as a valid means of capturing value-related information; for instance, a Business Model Canvas or DDD context map annotated with some additional text may serve as a mini-ConOps. Use of VBSEs from IEEE Std. 7000 is optional in ESE.

* You seem to use a certain analysis and design method terminology and meta-model. Where can I found information about it? 
  * *Answer:* We use the concepts from [DPR](https://github.com/socadk/design-practice-repository) here, slightly adopted. *Activities* yield *artifacts* and are supported by *techniques*. The artifacts are specified in certain *notations*, possibly supported by templates. The term *practices* refers to all method content that can be, well, practiced (used, that is); two practice types are activities and artifacts.

* How does ESE relate to and use existing documentation templates such as arc42?
  * *Answer:* It is complementary and extends what is already there. Detailed information is work in progress (see Future Work information).

* There are many regulations in countries and organizations, compliance management often is in place. Why is value-based systems/software engineering still needed? What does ESE differently? 
  * *Answer:* Values can be brought forward by any stakeholder (group); both positive and negative ones exist, with the aim to promote responsible behavior (in contrast to just following rules). ESE pushes ethical thinking and designing into the developer mainstream, practitioners no longer have to pull it from the literature or online resources.
  
* What is in the method engineering backlog?
  * *Answer:* Our work-in-progress and [Future Work](/ESE-FutureWork.md) includes additional application examples, (possibly) showing yet more notations. We also plan to provide more elaborate Markdown templates for ESE and IEEE Std. 7000 artifacts once/when the method content has matured and reached a steady state.

* How can I contribute, for instance by reporting a question missing here?
  * *Answer:* See [Contributions](/contributing/) folder and readme.

## Acknowledgment

Version 1.0 of ESE was supported by the [Hasler Foundation](https://haslerstiftung.ch/en/welcome-to-the-hasler-foundation/).
