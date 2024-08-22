---
Scope: Entire system and project or parts
Phases: n/a, regularly
Roles: Entire team
Input: All artifacts created or updated since last retrospective
Output: Report
Abstraction/Refinement Level: All
---

Activity: *Value Retrospective*
-------------------------------
also known as Value-Enhanced Heartbeat Retrospective, 5L Retrospective 

### Context

Engineers strive to be effective and efficient. From time to time, it makes sense to check whether a team is doing the right things and is doing them right. In the context of ethical (and agile) software engineering, this includes not only business requirements but also [ethical values](/ESE-Glossary.md#ethical-value) and requirements resulting from them.

Retrospectives are an established Agile practice to periodically reflect on what happened and how the teamwork, methods and tooling can be improved. The concept is enhanced and extended for ESE (this project/repository). See entry in [Agile Glossary](https://www.agilealliance.org/glossary/heartbeat-retrospective/) for general motivation.


### Goal and Purpose

The approach and results of the value-based approach in ESE must be reviewed periodically (w.r.t efficiency and effectiveness).

> *As a team of agile practitioners, we want to reflect periodically whether we are doing the rights things and whether we are doing things right. There always is room and opportunity for improvement. Being concerned about ethics values, we want to improve our value-based engineering practices continuously.*

Advantages and benefits of a Value Retrospective include: 

* The activity is faithful to Agile values (see [FAQs](/ESE-FAQ.md)).
* Participation is motivating for all team members, learners and experienced ones wanting to give back.
* Continuous improvement is imperative when following IEEE Std. 7000, for instance for validation and verification purposes. The Transparency Management Process benefits from such reflective approach. For instance, one could compare early retrospective reports with later ones to observe improvements.

#### Link to IEEE 7000

Regular reviews and retrospectives can be seen as the ESE realization of the Transparency Management Process in IEEE Std. 7000 (Clause 11).


### Instructions 

*Hold a Value Retrospective regularly, involving the entire team and, optionally, representatives of external stakeholder groups.*

In addition to the other/usual questions in a retrospective, ask the following ones: 

1. Is the amount of effort that we invest in value-based engineering (aka value-sensitive design) adequate for the given business context, domain and application genre? 
2. Did we investigate business and system context, expressed in the [Concept of Operations (ConOps)](/ESE-Glossary.md#conops), in sufficient depth and breadth?
3. Is our [Value Register](/ESE-Glossary.md#value-register) candid, complete, and agreed upon? Which values do we want to keep? 
4. Have we given our Ethical Value Requirements (EVRs) adequate, sufficient weight and priority?
5. How long did it take us to resolve conflicts and find tradeoffs during design? 
6. What do we want to do differently in the next iteration, for instance in terms of value prioritization? What has been missing so far in terms of values and addressing them? What are our 4Ls (Liked, Learned, Lacked, Long For) regarding the Ethical Value Requirement (EVRs)? 
7. Has our Transparency Management Process been effective and efficient?  

You also may want to revisit the [Ethics Review](ESE-EthicalReview.md) results: 

* Do the ethics artifacts (ConOps, Value Register, [Ethical Value Requirements (EVRs)](/ESE-Glossary.md#evr), and [VBSRs](/ESE-Glossary.md#vbsr)) require updates because of new learnings?


### Example(s)

The Value Lead, the Senior Product Manager (also serving as User Advocate) and the System Expert that performed the [Story Valuation](ESE-StoryValuation.md) for the Lakeside Mutual story meet one week after the [Ethical Review](ESE-EthicalReview.md) meeting to reflect and discuss how they can improve. 

Their meeting minutes include: 

~~~
Value Retrospective for "Lakeside Mutual, Customer Self Service iteration"

## Liked 

* ESE raises awareness for ethical concerns
* It makes IEEE 7000 accessible
* Oppertunities to provide feedback and to contribute to ESE are available 

## Learned

* Business and user value is important, but so are ethical values
* Any method or practice can and should be adopted, here: DoR and DoD (this worked fine) 
* Conflict resolution is not easy

## Lacked 

* It is not always clear how much time to invest and what kind of output to produce
* More time, more appreciation by external stakeholders for the extra mile
* External consultancy, for instance to moderate Ethical Review meeting

## Long For

* More guidance regarding story valuation, to be developed over time, will improve consensus building
* More examples, both small and large, for instance, how to conduct value jams and how to document EVR/VBSR efficiently
* Will try the alternative notations values tree and value canvas in next iteration
* Community for experience exchange
~~~


### Hints and Pitfalls to Avoid

Note that this retrospective primarily focuses on the development team and how it can do better w.r.t. the team's values; reviewing whether the values of end users and other stakeholders are met is the purpose of the Ethical Review.

* Look for a strong, empathic moderator/facilitator (see performing roles below).
* Get all team members actively involved in the retrospective. Reflect from multiple perspectives, including but not limited to end users, product owner/manager, development team, operations staff. 
* Create an open, trusted atmosphere; retrospectives are not the right place for blame games.[^1]
* Reserve enough time for the ethics- and value-related part; run it as a separate meeting if other topics (tools, practices, etc.) take too much time and attention.
* Record the results in a team-internal space. Control access to it strictly; do not forget to remove access rights when a team member leaves.
* Run Value Retrospectives more often than other retrospectives when new to ESE, IEEE Std. 7000.
* Add questions about impact of software if you find the ones in ESE to be incomplete. For instance, the Proactive CARE (onsider, Analyze, Review, and Evaluate) process sketched on the [ACM ethics website](https://ethics.acm.org/wp-content/uploads/2021/03/Proactive-CARE-for-Computing-Professionals.pdf) ask several more.
  
[^1]: Is there any right place and time for them?


### Related Content

#### Performing Roles and Related Artifacts

* [Value Lead](/roles/ESE-ValueLead.md)
* Moderator
* All other [roles](/roles) listed in IEEE Std. 7000


#### Practices and Techniques

In alphabetical order (new/extended in ESE): 

* [Definition of Done](ESE-DefinitionOfDone.md)
* [Definition of Ready](ESE-DefinitionOfReady.md)
* [Ethical Review](ESE-EthicalReview.md)
* [Story Valuation](ESE-StoryValuation.md)


### More Information 

General retrospectives are covered extensively in books and online resources: 

* The glossary of the Agile Alliance has an entry for ["Heartbeat Retrospectives"](https://www.agilealliance.org/glossary/heartbeat-retrospective/).
* Liked, Learned, Lacked, Long For (4L) evolved from other types of retrospectives, see this [ online article ]( https://www.ebgconsulting.com/blog/the-4ls-a-retrospective-technique/) (from June 24, 2010).
* ["Ethically Aligned Design: First Edition Glossary"](https://standards.ieee.org/wp-content/uploads/import/documents/other/ead1e_glossary.pdf) (92 pages)

The Design Practice Repository/Reference (DPR) on [GitHub](https://github.com/socadk/design-practice-repository), on [LeanPub](https://leanpub.com/dpr) summarizes agile architecting practices such as user stories. 

*Excursion and request for feedback on ESE:* Value Retrospectives might also yield method evaluation feedback on ESE (this repository and its content). To perform a full evaluation, go to [this page](/experimentation/). Information on how to contribute to the project can be found [here](/contributing/CONTRIBUTING.md). 


### Data Provenance 

```yaml
title: "ESE activity: Ethics-Enabled Retrospective"
author: Olaf Zimmermann (ZIO)
date: "11, 13, 2023 (Source: Project ESE)"
copyright: The author, 2023 (unless noted otherwise). All rights reserved.
license: Creative Commons Attribution 4.0 International License
```

