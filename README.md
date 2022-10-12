[![](https://img.shields.io/badge/indico-event-b34810?style=flat&logoColor=white)](https://indico.cern.ch/event/1106990/)
[![](https://img.shields.io/badge/indico-contribution-087cfc?style=flat&logoColor=white)](https://indico.cern.ch/event/1106990/contributions/4991351/)
[![](https://img.shields.io/badge/HTML-poster-E34F26?style=flat&logo=HTML5&logoColor=white)](https://github.com/mbarbetti/poster-acat2022-hopaas)
<!--
[![](https://img.shields.io/badge/arXiv-2204.09947-B31B1B?style=flat&logoColor=white)](https://arxiv.org/abs/2204.09947)
[![](https://img.shields.io/badge/PoS-(CompTools2021)034-78a434?style=flat&logoColor=white)](https://pos.sissa.it/409/034)
-->


# Hyperparameter Optimization as a Service on INFN Cloud
in [*21st International Workshop on Advanced Computing and Analysis Techniques in Physics Research*](https://indico.cern.ch/event/1106990/)

> **Authors:**
>
> LHCb Collaboration, L. Anderlini [1], M. Barbetti [1,2]

> **Affiliations:**
> 1. Istituto Nazionale di Fisica Nucleare, Sezione di Firenze, via G. Sansonse 1, Sesto Fiorentino (FI), Italy
> 2. Department of Information Engineering, University of Florence, via Santa Marta, 3, Firenze, Italy


## Abstract
The simplest and often most effective way of parallelizing the training of complex Machine Learning models is to execute several training  instances on multiple machines, possibly scanning the hyperparameter space to optimize the underlying statistical model and the learning procedure. 
Often, such a meta learning procedure is limited by the ability of accessing  securely a common database organizing the knowledge of the previous and ongoing trials. Exploiting opportunistic GPUs provided in different environments represents a further challenge when designing such optimization campaigns. 
In this contribution we discuss how a set of REST APIs can be used to access a dedicated service based on INFN Cloud to monitor and possibly coordinate multiple training instances, with gradientless optimization techniques, via simple HTTP requests. The service, named *Hopaas* (Hyperparameter OPtimization As A Service), is made of web interface and sets of APIs implemented with a FastAPI back-end  running through Uvicorn and NGINX in a virtual instance of INFN Cloud. The optimization algorithms are currently based on Bayesian techniques as provided by Optuna. A Python front-end is also made available for quick prototyping. 
We present applications to hyperparameter optimization campaigns performed combining private, INFN Cloud and CINECA resources.