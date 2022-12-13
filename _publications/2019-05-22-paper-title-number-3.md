---
title: "Simulation Scheduling of Variable-Structure Systems in OpenModelica "
collection: publications
permalink: /publication/2022-11-24-paper-openmodelica-scheduling
excerpt: 'We propose and implement a generic scheduling frame-work for OpenModelica to eliminate the simulation code corresponding to inactive components in a system-level model. This framework allows the model developer to auto-generate models corresponding to the discrete behavior of the underlying system, and then schedule their simulations. [**Read More**](http://nayakpriyam.github.io/publication/2022-11-24-paper-openmodelica-scheduling)'
date: 2022-11-24
venue: 'Proceedings of Asian Modelica Conference 2022, Tokyo, Japan, November 24-25, 2022'

---
We propose and implement a generic scheduling frame-work for OpenModelica to eliminate the simulation code corresponding to inactive components in a system-level model. This framework allows the model developer to auto-generate models corresponding to the discrete behavior of the underlying system, and then schedule their simulations. It also provides a Scheduler library in the Modelica language to help the model developer easily generate the schedule. The benefit of this approach is demonstrated with and without real-time simulations of a batch distillation system. The proposed approach also helps implement a sequential modular simulation to arrive at initial guesses for flowsheets, whose equations can then be solved simultaneously using the standard, equationoriented, approach of Modelica.

[Download paper here](https://ecp.ep.liu.se/index.php/modelica/article/view/569)

Recommended citation: Paknikar, Rahul, Nikhil Sharma, Priyam Nayak, Kannan Moudgalya, and Bhaskaran Raman. "Simulation Scheduling of Variable-Structure Systems in OpenModelica." In Modelica Conferences, pp. 147-155. 2022.