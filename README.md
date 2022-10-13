[![](https://img.shields.io/badge/indico-event-b34810?style=flat&logoColor=white)](https://indico.cern.ch/event/1106990/)
[![](https://img.shields.io/badge/indico-contribution-087cfc?style=flat&logoColor=white)](https://indico.cern.ch/event/1106990/contributions/4991348/)
[![](https://img.shields.io/badge/HTML-poster-E34F26?style=flat&logo=HTML5&logoColor=white)](https://mbarbetti.github.io/poster-acat2022-lamarr/poster.html)
<!--
[![](https://img.shields.io/badge/arXiv-2204.09947-B31B1B?style=flat&logoColor=white)](https://arxiv.org/abs/2204.09947)
[![](https://img.shields.io/badge/PoS-(CompTools2021)034-78a434?style=flat&logoColor=white)](https://pos.sissa.it/409/034)
-->


# Lamarr: LHCb ultra-fast simulation based on machine learning models
in [*21st International Workshop on Advanced Computing and Analysis Techniques in Physics Research*](https://indico.cern.ch/event/1106990/)

> **Authors:**
>
> LHCb Collaboration, L. Anderlini [1], M. Barbetti [1,2], G. Corti [3], A. Davis [4], D. Derkach [5], N. Kazeev [5], A. Maevskiy [5], S. Mokhnenko [5], B. Siddi [6], Z. Xu [7]

> **Affiliations:**
> 1. Istituto Nazionale di Fisica Nucleare, Sezione di Firenze, via G. Sansonse 1, Sesto Fiorentino (FI), Italy
> 2. Department of Information Engineering, University of Florence, via Santa Marta, 3, Firenze, Italy
> 3. European Organization for Nuclear Research, CERN, Esplanade des Particules, Meyrin, Switzerland
> 4. Schuster Laboratory, University of Manchester, Oxford Rd, Manchester, M13 9PL, United Kingdom
> 5. High School of Economics (HSE) University, 20 Myasnitskaya st., Moscow 101000, Russia
> 6. Physics Department, University of Ferrara, Via G. Saragat, 1, Ferrara (FE), Italy
> 7. Laboratoire de Physique de Clermont, LPC, Université Clermont Auvergne, 4 Avenue Blaise Pascal, Clermont, France


## Abstract
Abut 90% of the computing resources available to the LHCb experiment has been spent to produce simulated data samples for Run 2 of the Large Hadron Collider at CERN. The upgraded LHCb detector will be able to collect larger data samples, requiring many more simulated events to analyze the data to be collected in Run 3. Simulation is a key necessity of analysis to interpret signal vs background and measure efficiencies. The needed simulation will far exceed the pledged resources, requiring an evolution in technologies and techniques to produce these simulated data samples. In this contribution, we discuss Lamarr, a Gaudi-based framework to speed-up the simulation production parametrizing both the detector response and the reconstruction algorithms of the LHCb experiment.
Deep Generative Models powered by several algorithms and strategies are employed to effectively parametrize the high-level response of the single components of the LHCb detector, encoding within neural networks the experimental errors and uncertainties introduced in the detection and reconstruction phases. Where possible, models are trained directly on real data, statistically subtracting any background components through weights application. 
Embedding Lamarr in the general LHCb Gauss Simulation framework allows to combine its execution with any of the available generators in a seamless way. The resulting software package enables a simulation process completely independent of the Detailed Simulation used to date.