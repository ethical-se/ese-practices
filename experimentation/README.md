# Evaluation/Validation of Ethical Software Engineering (ESE) Practices

*Note:* This is an intermediate version of the instructions for a controlled experiment and/or user survey.

## Preparation

* Download IEEE Std. 7000 from [IEEE Xplore](https://ieeexplore.ieee.org/document/9536679) (free after registration). It will serve as a reference, there is no need to read it in its entirety.
* Orient yourself in the ESE repository, starting with the [README](/README.md) file, and, optionally, [ESE FAQ](/ESE-FAQ.md).
* Decide on one of your recent or ongoing projects or products as a sample system.


## Instructions

1. Pick an epic or an INVEST-ready user story from the backlog of the sample system. Think about the ethical values for the development and production usage of the sample system that come to your mind and/or that you consider essential for it.   
2. Create and instantiate the [ESE activities and artifacts](/practices/README.md) step-by-step (one at a time):
    1. [Story Valuation](/practices/ESE-StoryValuation.md) of the epic:  
        a) pick one of the three valuation techniques  
        b) choose from the proposed notations/documentation templates  
    2. [Definition of Ready](/practices/ESE-DefinitionOfReady.md) for the epic and its user stories
    3. [Definition of Done](/practices/ESE-DefinitionOfDone.md), assuming that some design and implementation work has happened since the story became ready
    4. [Ethical Review](/practices/ESE-EthicalReview.md) of/for the results of analysis and design work so far
    5. [Value Retrospective](/practices/ESE-ValueRetrospective.md) reflecting on the previous steps 
3. Compare the artifacts that you created while applying ESE with those you would have (or have) created on the original project. Did your thinking and approach change?

*Additional hints for Step 2:* 

* If you miss information because your sample system is rather small, you may want to use your imagination and existing examples to come up with draft versions of the missing artifacts. For instance, you can start with the Definition of Ready and the Definition of Done in the Example sections of the respective practices. 
* Between Steps 2 and 3, a full development iteration (or sprint) takes place in reality; if you only want to experiment with ESE, it is ok to rapidly create some exemplary design artifacts that are good enough to be value-assessed. 
* Do not get confused between the class/template and the instance/artifact level; your sample project/product requires a DoD and DoR template or checklist, for instance, and each story (or epic) then fills out these templates to create instances of them. 
* Keep an eye on effort vs. benefit/value; the "Hints and Pitfalls to Avoid" sections of the practices/artifacts remind you to do so. Do not fill out a template completely just because it is there![^1]

[^1]: "If in doubt leave it out" is one of the general method adoption rules, see the end of [this blog post](https://ozimmer.ch/practices/2023/02/07/DesignPracticeRepositoryVersion14.html).


## Review Questions 

Please reflect and, ideally, let us know too: 

1. How useful and accurate did you find the five ESE practice descriptions? Can you comment on their size: too short, just right, too long?
2. Does ESE provide the right amount of background information about Agile practices and IEEE Std. 7000? Do their combination and linkage work for you? 
3. Which strengths, weaknesses, opportunities, and threats do you see for the adoption of ESE in practice? How can the weaknesses and threats be overcome? 

Any other feedback on method content and its presentation (including repository organization) will also be appreciated. 

[CONTIBUTING.md](/contributing/) specifies how to get provide feedback and how to contribute.

*November 13, 2023*  
*[ZIO](https://medium.com/olzzio) aka Olaf Zimmermann*


## Acknowledgment

Version 1.0 of ESE was supported by the [Hasler Foundation](https://haslerstiftung.ch/en/welcome-to-the-hasler-foundation/).
