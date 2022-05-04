---
title: 'Natural Language Processing to Assure the Quality of User Stories (Michiel Blommaert)'
date: '2018-06-13T13:29:45+00:00'
author: 'Geert Poels'
layout: post
---

**Context**

In Agile Software Engineering, working software is valued over comprehensive documentation (http://agilemanifesto.org). Currently, practitioners of agile development practices often misinterpret this as ‘no documentation’. Consequently, user stories are almost the only kind of requirements documentation maintained in the application of agile development methods.

A user story describes a feature required to be provided by a software system in terms of a standard template structure. User stories are always formulated from the perspective of the person that desires the feature. A typical template for formulating user stories is:

As a *type of user*, I want *some goal* so that *some reason*

For example, related to requirements for a car navigation system, a user story could be:

*As a driver, I want to be notified of traffic jams on my route, so that I avoid losing time.*

Past research has shown that the documentation as a separate user story of each system feature desired by some system stakeholder might cause problems when at a later stage the agile development team loses the high-level view of the various system functions and their interaction. The problem gets magnified when the composition of the team changes, e.g., when new members join the team and need to comprehend the high-level architecture of the system under development. Even for moderately complex software, the number of user stories easily exceeds human capacity of overview and understanding. Furthermore, the more user stories are created, the more details are required in the acceptance criteria which are used for testing the system. Acceptance criteria are metrics that define when the system’s functionality is acceptable in response to a user story. If user stories are not integrated and aligned with each other, they create ambiguity, making it harder to decide when a system meets its requirements.

To alleviate the problems mentioned above, the use of conceptual models is suggested. Conceptual models are visual representations that are commonly used for understanding, analyzing and communicating system requirements. In ‘traditional’ (i.e., not agile) software development methods, a conceptual model is a graphical model with well-defined syntax and semantics that describes the domain to be supported by a software system (e.g., the domain of car navigation). This description is independent of the manner in which the software system is implemented. In other words, a conceptual model captures the function of a domain (e.g., how to use car navigation to achieve a purpose) and its behavior (e.g., how car navigation is used during a car trip), as well as its construction (e.g., what components does car navigation consist of and how are they related -car, GPS satellite network, GPS receiver, etc.) and its operation (e.g., GPS satellites broadcast signals about their current time and position), but does not prescribe decisions that should be left to the discretion of system developers (e.g., which track algorithm the GPS receiver runs to calculate the location, speed and direction of the car).

What is currently missing in the state-of-the-art is the automated generation of conceptual models that show both the functional (de)composition of the domain (i.e., function and behavior)) and the constructional (de)composition of the domain (i.e., construction and operation). Further, there is no empirical study that investigates the costs (e.g., effort to understand the conceptual model) and benefits (e.g., increased understanding of dependencies and other relationships between user stories) of using conceptual models generated from user stories. In other words, showing feasibility of automated generation of conceptual models from user stories is one thing; demonstrating the economic value of such approach in terms of increased quality and productivity of agile software development is something else, at least equally important for the valorization of the research.

**Thesis description**

At UGentMIS we initiated a line of research in which we investigate, together with researchers from Saint Louis University (USA) and a high-tech USA company, whether Natural Language Processing (NLP) techniques could be used to automatically generate conceptual models from user stories. The NLP-based generation of models has proven to be a challenging area, giving rise to many research questions, some of which we wish to address via master dissertation research. The current thesis topic results from this initiative.

This thesis will look into techniques to assure the quality of user stories. The success of NLP heuristics used for the recognition of concepts in user stories that are needed to build conceptual models, strongly depends on the quality of the user stories. In this context, quality refers to how well the user story fits the user story template, i.e., the correctness and completeness of filling the user story template. A starting point is the technique developed by Lucassen et al. (2016) and later formalised in the GRIMM method developed at Utrecht University (contacts will be provided by the thesis supervisor).

The purpose of the thesis is to evaluate how this technique (and possibly other methods that are discovered through literature study) can be applied as a pre-processing step to the US2CM (User Story To Conceptual Model) text-to-model algorithm that we are developing at UGentMIS – SLU. The eventual result of the thesis is a tailoring of the quality assurance technique to the specific text-to-model algorithm that we develop and an assessment of the improvement in terms of model quality that results from the pre-processing (as compared to a situation without pre-processing). We expect results to be publishable and invite the thesis student to co-author any paper resulting from the thesis.

**References**

Lucassen, G., Dalpiaz, F., van der Werf, J.M.E., and S. Brinkkemper. 2016. Improving agile requirements: the quality user story framework and tool. Requirements Engineering (21:3), pp. 383-403