
# Ethical Software Engineering (ESE)

*Quick links:* (1) [Story Valuation](./practices/ESE-StoryValuation.md), (2) [Ethical Review](./practices/ESE-EthicalReview.md), (3) two-way [Practice-Process Mappings](./ESE-BackgroundInformation.md#from-agile-practices-to-ieee-std-7000-concepts) (4) [Glossary](ESE-Glossary.md) (5) [FAQs](ESE-FAQ.md)  
*Sibling repository:* Value-Driven Analysis and Design, seven-step [process](https://ethical-se.github.io/value-driven-analysis-and-design/process/), two additional [practices](https://ethical-se.github.io/value-driven-analysis-and-design/practices/).

## ESE Goals  

Ethical Software Engineering (ESE) is for you if: 

1. You see yourself as a socially *responsible software engineer*. <!--, not just a "code monkey".[^1] -->
2. You want to *manage and mitigate the risk* that a project or product development effort and the software under construction may have undesired and/or unexpected and/or unjustified effects for one or more of its stakeholder groups.  
3. You look for a set of *essential<!--, as-light-as-possible--> practices that help to adopt IEEE Std. 7000*. 

<!-- [^1]: "Code monkey" is a term used by Martin Fowler in presentations on the topic. We use it here under the assumption that monkeys will not feel discriminated by this term. -->

<!-- TODO (v2) cite from CoC preamble (see ETHICOMP presentation notes) -->
<!-- TODO (v2) show a filled-out Value Story too, as figure? -->

Let's assume that a development team has been assembled to enhance an online shop with a same-day delivery capability. Different stakeholders exist, and their project goals differ too:

![Motivating example: ethical and other values in a same-day delivery scenario](/images/ETHICOMP2024-SDDExample.png)

ESE aims at answering the questions and managing value conflicts systematically. It does not mandate or enforce any particular values, but provides a framework for value-based, ethical software engineering.

## ESE Approach 

ESE targets any software engineer[^2] who wishes to create ethically valuable software, agile teams in particular. See [roles folder](./roles/README.md) for user stories, shared with the sibling [Value-Driven Analysis and Design (VDAD)](https://ethical-se.github.io/value-driven-analysis-and-design/user-stories) project. 

Principles that guided the design of ESE include:[^1]

* *Synergies:* A value- and risk-based approach to design is very much at the heart of agile methods; for instance, [Extreme Programming](https://www.agilealliance.org/glossary/xp) aims at balancing cost, time, quality and scope variables. <!-- Sources: "Extreme Programming Explained" by Kent Beck and the "iron cross" discussion in "Clean Agile" by Robert C. Martin -->  
* *Dual relation:* Agile practices may promote social responsibility and ethical behavior, but may also harm ethical values. The devil is in the detail, software usage context matters. 
* *Novelty:* The topic of ethical values has not been discussed much in Agile practices so far.[^3] The Agile Alliance has a [Code of Conduct](https://www.agilealliance.org/code-of-conduct/). And a blog post on [coaching ethics](https://www.agilealliance.org/identifying-a-code-of-ethical-conduct-for-agile-coaching/) made it to the top 10 of 2022 (Agile Alliance).

[^1]: An ETHICOMP 2022 paper, "From the Page to Practice: Support for Computing Professionals Using a Code of Ethics", makes the case for a proactive approach. It presents a Consider, Analyze, Review, Evaluate (CARE) process. See the [Bibliography](ESE-Literature.md) page.

[^2]: We use the term "software engineer" in a broad sense here, including roles such as requirements engineer, architect, developer, tester, operator and maintainer. The entire software development lifecycle is in scope, with special emphasis on analysis and design.
 
[^3]: For instance, search for terms such as "ethics" on the [website](https://www.agilealliance.org/) of the Agile Alliance.

ESE lets [IEEE Std. 7000](https://ieeexplore.ieee.org/document/9536679) meet Agile practices (note: access to IEEE Std. 7000 is free after registration for IEEE Xplore):

![Agile and ESE Practices per IEEE 7000 stage and phase](/images/ESE-OverlayIEEE7000.png)


## ESE Repository Content Navigation 

ESE provides new and/or enhanced [practices](./practices/) (i.e., activities and artifacts):

* [Story Valuation](./practices/ESE-StoryValuation.md) activity, ***a good place to get started with ESE***
* [Ethical Review](./practices/ESE-EthicalReview.md) report and meeting
* Extended, value-enhanced [Definition of Ready](./practices/ESE-DefinitionOfReady.md) artifact
* Extended, value-enhanced [Definition of Done](./practices/ESE-DefinitionOfDone.md) artifact
* [Value Retrospective](./practices/ESE-ValueRetrospective.md) activity, inspired by and complementing other forms of retrospectives.

Other folders and pages in this repository include:

* [Roles directory](/roles) (not fully populated at present)
* [Experimentation](/experimentation) instructions (method validation)
* [Future work](/ESE-FutureWork.md)

Other content is linked in the directory-level index pages.


## Prerequisite Knowledge 

Experience with the Agile practices that ESE applies, extends or complements is welcome and useful but not strongly required; links and examples provide opportunities to catch up.

Working with ESE (the content of this repository) does not assume that you have read the IEEE Std. 7000. It is helpful but not required to be familiar with selected concepts and processes; these are introduced and/or referenced as needed. 
The [Background Information](ESE-BackgroundInformation.md) page provides value comparisons and mappings from IEEE Std. 7000 to Agile concepts and practices (and back).

## Background Information 

What are (ethical) values? Which ones matter? Our [Glossary](ESE-Glossary.md)  references the definitions of the terms [value](/ESE-Glossary.md#value) and [ethical value](/ESE-Glossary.md#ethical-value) from IEEE Std. 7000; the [Merriam-Webster Dictionary](https://www.merriam-webster.com/dictionary/ethic) defines the term "ethic".

The following figure shows three different meanings of the term "value", depending on the viewpoint taken:

![](/images/ESE-ValueHierarchy.png)

For additional motivation for ethical software engineering and terminology clarification, please refer to ["Are Programmers Ethically (and Legally) Responsible for Their Code?"](https://thenewstack.io/are-programmers-ethically-and-legally-responsible-for-their-code/), an article by Jennifer Riggins on The New Stack (Aug 16, 2018).

ESE was featured at the ETHICOMP 2024 conference: 

* Conference presentation [""Bringing Ethical Values into Agile Software Development""](https://ozimmer.ch/assets/presos/ZIO-ESEAtETHICOMPv10p.pdf) (PDF, 23 slides)
* Peer-reviewed [extended abstract](https://dialnet.unirioja.es/descarga/articulo/9326119.pdf) (PDF, 3 pages)
* Full proceedings [paper](resources/ESE-ETHICOMP2024FullPaperAuthorsCopyV101.pdf) (PDF, 10 pages)

Several additional resources are available within ESE: 

* A [Glossary](ESE-Glossary.md) defines and explains terms in IEEE Std. 7000, Agile, ESE.
* A collection of [Frequently Asked Questions (FAQs)](ESE-FAQ.md) is available.
* Literature and related work appear in a [Bibliography](ESE-Literature.md).


## Evaluation and Feedback 

See [experimentation](/experimentation/) folder and README.

*July 28, 2025*  
*[ZIO](https://ozimmer.ch/about/)*


## Acknowledgments

Bärbel Bohr, Mirko Stocker and Stefan Kapferer contributed to the ESE content via discussion input, experimenation and/or review feedback before its public release. The attendees of the ETHICOMP 2024 presentation on ESE Version 1.0, as well as other conference attendees, provided 
valuable feedback, incorporated in the current version. Thank you very much indeed!

Version 1.0 of ESE was supported by the [Hasler Foundation](https://haslerstiftung.ch/en/welcome-to-the-hasler-foundation/).
