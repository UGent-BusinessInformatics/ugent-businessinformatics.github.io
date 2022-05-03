---
id: 3047715
title: 'Enhancing Agile Development through Modelling of User Stories (Emma Willard &#038; Axelle Pysson)'
date: '2018-08-01T08:41:38+00:00'
author: 'Geert Poels'
layout: post
guid: 'http://www.mis.ugent.be/?p=3047715'
permalink: /enhancing-agile-development-through-modelling-of-user-stories/
categories:
    - 'Master Dissertations 2020'
    - 'Master Dissertations Geert Poels 2020'
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

There have been past attempts at text-to-model transformations of user stories. Lin et al. (2014) present an approach were an analysis of user stories is used to refine the top-level goals in a given goal model, i.e., a conceptual model that describes a domain in terms of its stakeholders (which typically includes the software system itself), their goals, and how these stakeholders depend on each other for goal achievement. Mesquita et al. (2015) succeeded in the automatic generation of skeletons of goal models (articulated in the i\* language) from user stories. Robeer et al. (2016) built a tool that automatically generates an ontological model of the domain (articulated as an OWL ontology) from user stories. The ontological model shows domain concepts and relationships extracted from the user stories through the use of state-of-the-art Natural Language Processing (NLP) techniques.

The purpose of the thesis is to assess the application of text-to-model transformation of user stories in Agile Software Engineering. How can Natural Language Processing of user stories enhance the process of Agile development? To investigate this research question, the thesis will look into past and current techniques (including those developed in the project with SLU/Testing Algorithms), apply them to example sets of user stories and evaluate their application potential in enhancing requirements engineering. If results are promising, a scientific publication will be extracted from the thesis work, co-authored by the thesis student.

**References**

Lin, J., Yu, H., Shen, Z., and Miao, C. 2014. Using goal net to model user stories in agile software development. In: Proceedings of IEEE/ACIS International Conference on Software Engineering, Artificial Intelligence, Networking and Parallel/Distributed Computing. Las Vegas, IEEE, pp. 1-6.

Mesquita, R., Jacqueira, A., Agra, C., Lucena, M., and F. Alencar. 2015. US2StarTool: generation i\* models from user stories. In: Proceedings of the International i\* Workshop (iStar). pp. 103-108.

Robeer, M., Lucassen, G., van der Werf, J.M.E., Dalpiaz, F., and S. Brinkkemper. 2016. Automated extraction of conceptual models from user stories via NLP. In: Proceedings of the 24th International Conference on Requirements Engineering. IEEE. pp. 196-205.