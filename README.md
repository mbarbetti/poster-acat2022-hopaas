# Hyperparameter Optimization as a Service on INFN Cloud
in [*21st International Workshop on Advanced Computing and Analysis Techniques in Physics Research*](https://indico.cern.ch/event/1106990/) (ACAT 2022)

[![](https://img.shields.io/badge/indico-event-c89e6c?style=flat&logoColor=white)](https://indico.cern.ch/event/1106990/)
[![](https://img.shields.io/badge/indico-contribution-087cfc?style=flat&logoColor=white)](https://indico.cern.ch/event/1106990/contributions/4991351/)
[![](https://img.shields.io/badge/HTML-poster-E34F26?style=flat&logo=HTML5&logoColor=white)](https://mbarbetti.github.io/poster-acat2022-hopaas/poster.html)
[![](https://img.shields.io/badge/PDF-poster-EC1C24?style=flat&logo=Adobe%20Acrobat%20Reader&logoColor=white)](https://indico.cern.ch/event/1106990/contributions/4991351/attachments/2532524/4357741/hopaas_poster_acat2022.pdf)
[![](https://img.shields.io/badge/arXiv-2301.05522-B31B1B?style=flat&logoColor=white)](https://arxiv.org/abs/2301.05522)
<!--
[![](https://img.shields.io/badge/J%20Phys:%20Conf%20Ser-(1525)012097-236fb5?style=flat&logoColor=white)](https://dx.doi.org/10.1088/1742-6596/1525/1/012097)
[![](https://img.shields.io/badge/PoS-(CompTools2021)034-78a434?style=flat&logoColor=white)](https://pos.sissa.it/409/034)
-->

## Abstract
The simplest and often most effective way of parallelizing the training of complex machine learning models is to execute several training  instances on multiple machines, possibly scanning the hyperparameter space to optimize the underlying statistical model and the learning procedure. 
Often, such a meta learning procedure is limited by the ability of accessing  securely a common database organizing the knowledge of the previous and ongoing trials. Exploiting opportunistic GPUs provided in different environments represents a further challenge when designing such optimization campaigns. 
In this contribution we discuss how a set of RestAPIs can be used to access a dedicated service based on INFN Cloud to monitor and possibly coordinate multiple training instances, with gradientless optimization techniques, via simple HTTP requests. The service, named Hopaas (_Hyperparameter OPtimization As A Service_), is made of web interface and sets of APIs implemented with a FastAPI back-end  running through Uvicorn and NGINX in a virtual instance of INFN Cloud. The optimization algorithms are currently based on Bayesian techniques as provided by Optuna. A Python front-end is also made available for quick prototyping. 
We present applications to hyperparameter optimization campaigns performed combining private, INFN Cloud and CINECA resources.

> **Authors:**
>
> M. Barbetti [1,2], L. Anderlini [2]

> **Affiliations:**
> 1. Department of Information Engineering, University of Florence, via Santa Marta, 3, Firenze, Italy
> 2. Istituto Nazionale di Fisica Nucleare, Sezione di Firenze, via G. Sansonse 1, Sesto Fiorentino (FI), Italy

## Cite us
Are you using Hopaas in your research project? Please cite us!

> M. Barbetti and L. Anderlini, **Hyperparameter Optimization as a Service on INFN Cloud**, in _21st International Workshop on Advanced Computing and Analysis Techniques in Physics Research (ACAT 2022)_, [arXiv:2301.05522](https://arxiv.org/abs/2301.05522)

```bibtex
@inproceedings{hopaas:2023,
    author = "Barbetti, Matteo and Anderlini, Lucio",
    title = "{Hyperparameter Optimization as a Service on INFN Cloud}",
    booktitle = "{21st International Workshop on Advanced Computing and 
                Analysis Techniques in Physics Research (ACAT 2022)",
    eprint = "2301.05522",
    archivePrefix = "arXiv",
    primaryClass = "cs.DC",
    month = "1",
    year = "2023"
}
```

## Credits
Poster project based on [cpitclaudel/academic-poster-template](https://github.com/cpitclaudel/academic-poster-template). Poster webpage hosted by [GitHub page](https://pages.github.com).
