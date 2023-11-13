## Future Work 

### Mappings: From Context and Analysis to Design 

The following table indicates when and where certain ethical values (from Annex G of IEEE Std. 7000) require particular attention: <!-- TODO (L) use bullet list with value explanations from Annex G, following the table, to carve out VBSRs from EVRs that shine through; makes table and phase/layer mapping more precise -->

| Core/Overarching Value | Example/Instance | [SDLC](https://www.tutorialspoint.com/sdlc/sdlc_overview.htm#) Phase | Logical Layer (UIL, BLA, DAS) |
|-|-|-|-|
| Autonomy | tbc | tbd | tbc | 
| Care | tbc  | all | BLA |
| Control | tbc | design | UIL, BLA |
| Fairness | tbc | all | BLA |
| Inclusiveness | tbc | analysis | BLA |
| Innovation | tbc | analysis, design | all |
| Perfection | tbc | all | all |
| Privacy | tbc | all | UIL, DAS |
| Respect | tbc | analysis, design | UIL, BLA |
| Sustainability | tbc | all | all |
| Transparency | tbc | all | UIL, DAS |
| Trust | tbc | all | BLL, DAS |

*Legend:* UIL = User Interface Layer, BLA = Business Logic and Algorithms, DAS = Data Access and Data Storage Layer. SDLC phases as defined in ISO standards such as ISO/IEC/IEEE12207. 

*work in progress, not sure about SDLC (Software Development Lifecycle)*

<!-- TODO (L) could provide more value mapping tables: revisit Scrum and XP (via B. Meyer book? Clean Agile?) could also create a Value Register for ASD (DPR method/repo as SOI?) -->

| Core/Overarching Value | Level 1 Value | Application Genre | Domain Pattern |
|-|-|-|-|
| Autonomy | tbc | System of Engagement (SoE) | See C. Lilienthal's presentation "Domain-Driven Transformation", summarized in [TAMLE event report](https://medium.com/olzzio/notes-from-the-architecture-and-modeling-learning-event-part-2-28287a7f13b0) | 
| Care | tbc  | SoE |  |
| Control | tbc | SoE, System of Record (SoR) | |
| Fairness | tbc | all | |
| Inclusiveness | SoR | analysis | |
| Innovation | tbc | all | |
| Perfection | tbc | all | |
| Privacy | tbc | all | |
| Respect | tbc | all | |
| Sustainability | tbc | all | |
| Transparency | tbc | all | |
| Trust | tbc | all |  |

Examples of application genres include Web shops, risk management applications, billing systems, CRM systems, help desk/user support systems, social networks, etc; SoE stands for System of Engagement and SoR is System of Record. 


### Notations

A *value canvas* is one way of organizing the output of this activity, providing an alternative to the table-text notation suggested above (under "Instructions" and "Example"): 

![ESE/IEEE 7000 Value Canvas (Meta Model)](/images/ESE-ValueCanvas.png)


### Additional FAQs

* IEEE Std. 7000 is about systems engineering, a superset of software engineering. Does ESE prioritize any particular values? 
  * *Answer:* See the following table (work in progress, subject to change):

| Core/Overarching Value | Meaning, Means | Priority (H/M/L) | Comments (+, o, -) |
|-|-|-|-|
| Autonomy | See Story Valuation practice page | H in ESE | |
| Care | e.g. HCID, UX  | | |
| Control | Three types/levels: info, decision, behavior <!-- see TODO handwritten notes --> | H in ESE | |
| Fairness | | H in ESE | |
| Inclusiveness |  |  | |
| Innovation |  |  | |
| Perfection |  |  | |
| Privacy | TODO: See definition in IEEE 7000 Std. | H in ESE | |
| Respect | TODO: Friendly and helpful error messages, etc. | H in ESE | |
| Sustainability | |  | |
| Transparency | TODO: See definition in IEEE 7000 Std. | H in ESE | |
| Trust | TODO: See definition in IEEE 7000 Std. | H in ESE | |


### Misc

Future directions for ESE may include: 

* Provide more application/adoption [examples](/examples/)
* Enhance Markdown [templates](/templates/) and integrate ESE into description formats such as arc42
* Validate all method content further (see [experimentation](/experimentation/) page)
* Improve existing or add new notations, e.g. Value Tree (already featured in an example), Value Canvas or Value Mapping <!-- [O] QOC+, bipartite graph? --> 
* Discuss what Enterprise Architecture Management (EAM) can add (TOGAF, Zachman, etc.): ConOps input?
* Scaling ESE: many epics and stories, large and heterogeneous stakeholder landscape, many and many conflicting values, ...  
* Look at other agile practices: story points, planning poker?
* More emphasis on design decisions: ethical decision making and recording, value-based decision rationale ("Y+", extension to MADR template and its explanations)
* More emphasis on design process and phases (SOI as value bearer, value disposition): map software quality attributes to values and back (Annex G), value-based architectural modeling, architectural components supporting Transparency Management <!-- [O] extension to ADD? QOC? Decision making methods? -->
* *to be continued*


## Acknowledgment

This work was funded by the [Hasler Foundation](https://haslerstiftung.ch/en/welcome-to-the-hasler-foundation/).
