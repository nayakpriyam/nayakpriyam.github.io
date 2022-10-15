---
title: "Implementation of a Property Database and Thermodynamic Calculations in OpenModelica for Chemical Process Simulation"
collection: publications
permalink: /publication/2019-02-20-paper-thermo
excerpt: 'An attempt has been made to enhance the thermodynamic capability of the general purpose modeling and simulation environment OpenModelica. The property database ChemSep and the thermodynamic algorithms of DWSIM are made available in OpenModelica. [**Read More**](http://nayakpriyam.github.io/publication/2019-02-20-paper-thermo)'
date: 2019-02-20
venue: 'Industrial & Engineering Chemistry Research'

---
An attempt has been made to enhance the thermodynamic capability of the general purpose modeling and simulation environment OpenModelica. The property database ChemSep and the thermodynamic algorithms of DWSIM are made available in OpenModelica. The following three approaches, listed in the order of increasing computational efficiency, are attempted in this work: Python-C API, socket programming, and a native port. The most efficient method of native port is adopted to make available NRTL, Peng–Robinson, UNIFAC, and UNIQUAC algorithms in OpenModelica. Through several examples, OpenModelica results are compared with Aspen Plus, indicating a good match in all cases. This work is released as an open source to enhance the collaboration among chemical engineers.

[Download paper here](https://pubs.acs.org/doi/full/10.1021/acs.iecr.8b05147)

Recommended citation: Jain, Rahul, Priyam Nayak, Rahul A. S, Pravin Dalve, Kannan M. Moudgalya, P. R. Naren, Daniel Wagner, and Peter Fritzson. "Implementation of a Property Database and Thermodynamic Calculations in OpenModelica for Chemical Process Simulation." Industrial & Engineering Chemistry Research 58, no. 18 (2019): 7551-7560.