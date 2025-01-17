---
authors: [harry-scells, jimmy, guido-zuccon]
title: "Big Brother: A Drop-In Website Interaction Logging Service"
venue: Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval
year: 2021
pdf: 
projects: [] 
redirect_from: /bigbro
links:
 - url: https://github.com/hscells/bigbro
   name: GitHub
---

**Pre-print coming soon**

Fine-grained logging of interactions in user studies is important for studying user behaviour, among other reasons. However, in many research scenarios, the way interactions are logged are usually tied to a monolithic system. We present a generic, application-independent service for logging interactions in web-pages, specifically targetting user studies. Our service, Big Brother, can be dropped-in to existing user interfaces with almost no configuration required by researchers. Big Brother has already been used in several user studies to record interactions in a number of user study research scenarios, such as lab-based and crowdsourcing environments. We further demonstrate the ability for Big Brother to scale to very large user studies through benchmarking experiments. Big Brother also provides a number of additional tools for visualising and analysing interactions.

Big Brother significantly lowers the barrier to entry for logging user interactions by providing a minimal but powerful, no configuration necessary, service for researchers and practitioners of user studies that can scale to thousands of concurrent sessions. We have made the source code and releases for Big Brother available for download at [https://github.com/hscells/bigbro](https://github.com/hscells/bigbro).