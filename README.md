# BMIElectromagneticEmissions
Electromagnetic emissions of a Brain-Machine Interface developed by Monash Vision Group

This repository provides the COMSOL files for the manuscript entitled "A model for assessing the electromagnetic safety of an inductively coupled, modular brain-machine interface", by Julian Szlawski, Timothy Feleppa, Anand Mohan, Yan T. Wong, and Arthur J. Lowery. We provide this model to members of the scientific and medical device development community in the hopes that it can be applied to a multitude of different BMI configurations that utilise inductive links.

To save computational time, the geometry has been truncated. The original and truncated geometry can be found in the project file. When solving for SAR and Bioheating, these components have been split into two different studies and must be solved sequentially. To solve for SAR, disable the Bioheat Transfer module and the Multiphysics node, and solve Study 1: SAR only. After the solution has been generated, enable the Bioheat Transfer module and the Multiphysics node, then solve Study 2: Temperature only. 
