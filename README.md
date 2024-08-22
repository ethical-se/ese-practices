# ethical-software-engineering (ESE)
*TL;DR:* [IEEE Std. 7000](https://ieeexplore.ieee.org/document/9536679) meets Agile practices
(note: access to IEEE Std. 7000 is free after registration for IEEE Xplore).

![Agile and ESE Practices per IEEE 7000 stage and phase](/images/ESE-OverlayIEEE7000.png)

*Quick links:* (1) [Story Valuation](./practices/ESE-StoryValuation.md), (2) [Ethical Review](./practices/ESE-EthicalReview.md), (3) two-way [Practice-Process Mappings](./ESE-BackgroundInformation.md#from-agile-practices-to-ieee-std-7000-concepts) (4) [Glossary](ESE-Glossary.md) (5) [FAQs](ESE-FAQ.md)

## Motivation

<!-- TODO (v2) cite form CoC preamble (see ETHICOMP presentation notes) -->

Ethical Software Engineering (ESE) is for you if: 

1. You see yourself as a socially responsible software engineer. <!--, not just a "code monkey".[^1] -->
2. You see the risk that the software under construction may have undesired and/or unexpected and/or unjustified effects for one or more of its stakeholder groups and want to manage and mitigate this risk.  
3. You look for a set of essential, as-light-as-possible practices that increase the chances of your project or product development effort becoming compliant with IEEE Std. 7000. 

<!-- [^1]: "Code monkey" is a term used by Martin Fowler in presentations on the topic. We use it here under the assumption that monkeys will not feel discriminated by this term. -->

ESE targets any software engineer[^2] who wishes to create ethically valuable software, agile teams in particular. Its motivating themes are:[^1]

* *Synergies:* A value- and risk-based approach to design is very much at the heart of agile methods; for instance, [Extreme Programming](https://www.agilealliance.org/glossary/xp) aims at balancing cost, time, quality and scope variables. <!-- Sources: "Extreme Programming Explained" by Kent Beck and the "iron cross" discussion in "Clean Agile" by Robert C. Martin -->  
* *Dual relation:* Agile practices may promote social responsibility and ethical behavior, but may also harm ethical values. The devil is in the detail, software usage context matters. 
* *Novelty:* The topic of ethical values has not been discussed much in Agile practices so far.[^3] The Agile Alliance has a [Code of Conduct](https://www.agilealliance.org/code-of-conduct/). And a blog post on [coaching ethics](https://www.agilealliance.org/identifying-a-code-of-ethical-conduct-for-agile-coaching/) made it to the top 10 of 2022 (Agile Alliance).

[^1]: An ETHICOMP 2022 paper, "From the Page to Practice: Support for Computing Professionals Using a Code of Ethics", makes the case for a proactive approach. It presents a Consider, Analyze, Review, Evaluate (CARE) process. See the [Bibliography](ESE-Literature.md) page.

[^2]: We use the term "software engineer" in a broad sense here, including roles such as requirements engineer, architect, developer, tester, operator and maintainer. The entire software development lifecycle is in scope, with special emphasis on analysis and design.
 
[^3]: For instance, search for terms such as "ethics" on the [website](https://www.agilealliance.org/) of the Agile Alliance.

But what are ethical values? Our glossary references the definitions of the terms [value](/ESE-Glossary.md#value) and [ethical value](/ESE-Glossary.md#ethical-value) from IEEE Std. 7000; the [Merriam-Webster Dictionary](https://www.merriam-webster.com/dictionary/ethic) defines the term "ethic".
The following figure shows three different meanings of the term "value", depending on the viewpoint taken:

![](/images/ESE-ValueHierarchy.png)

For additional motivation for ethical software engineering and terminology clarification, please refer to ["Are Programmers Ethically (and Legally) Responsible for Their Code?"](https://thenewstack.io/are-programmers-ethically-and-legally-responsible-for-their-code/), an article by Jennifer Riggins on The New Stack (Aug 16, 2018).

<!--
TODO (v2) add section 

## Goals and Approach

Goals and non-goals: 

* + raise awareness, - allow for ethics washing 
* + stimulate discussions, - over-simplify or reduce time to think and decide 
* + education aid, - command/control tool 
* + decision support, - decision making

Approach: "attention and reflection" are required to become a responsibleSWE; ESE provides motivation, examples, pointers, TODOs for team/roles; but no simple workflow (or even answers) or set of checkbox questions (topic is too complex and too "wicked" for that) or predefine value catalogs with right-wrong intructions, in the spirit of "positive responsibility" (John Ladd, 1993). 
-->


## Repository Navigation 

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


## Prerequisite Knowledge and Background Information

*Working with ESE (the content of this repository) does not assume that you have read the IEEE Std. 7000 end to end.* It is helpful but not required to be familiar with its concepts and processes; these are introduced and/or referenced as needed. 

Experience with the Agile practices that ESE applies, extends or complements is welcome and useful but not strongly required; links and examples provide opportunities to catch up.

The [Background Information](ESE-BackgroundInformation.md) page provides value comparisons and mappings from IEEE Std. 7000 to Agile concepts and practices (and back).


## Glossary

The [Glossary](ESE-Glossary.md) defines and explains terms in IEEE Std. 7000, Agile, ESE.


## Frequently Asked Questions

A collection of [Frequently Asked Questions (FAQs)](ESE-FAQ.md) is available.


## Literature and Related Work

See [Bibliography page](ESE-Literature.md).


## Evaluation and Feedback 

See [experimentation](/experimentation/) folder and README.

*August 21, 2024*  
*[ZIO](https://medium.com/olzzio) aka Olaf Zimmermann*


## Acknowledgments

Bärbel Bohr, Mirko Stocker and Stefan Kapferer contributed to the ESE content via discussion input, experimenation and/or review feedback before its public release. The attendees of the ETHICOMP 2024 presentation on ESE Version 1.0, as well as other conference attendees, provided 
valuable feedback, incorporated in the current version. Thank you very much indeed!

Version 1.0 of ESE was supported by the [Hasler Foundation](https://haslerstiftung.ch/en/welcome-to-the-hasler-foundation/).
