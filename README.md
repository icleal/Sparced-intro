# Welcome
The purpose of this page is to share the basic knowledge required to operate the SPARCED model. We do not intend for this page to be a comprehensive guide to the SPARCED model. Instead, we hope this will serve as a self-contained roadmap for future Clemson University Creative Inquiry (C.I.) students to familiarize themselves with the model efficiently and begin to run SPARCED simulations independently.
# Layout
- PanCancer/ Bouhadou <br /> - The origin of SPARCED <br /> -How to set up SPARCEDon the command line <br /> -How to run it on Palmetto
#  Pan cancer <h6> 
To entirely understand what the SPARCED model is, it is best learn what it came from.  This would be the PAN cancer model.  The official paper can be found [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5886578/).  This is a mechanistic model of Cancer in a MCF10A cell, which is a non-tumorigenic epithelial cell line.  The model is an "integrated system of ordinary differential equations"  which was coded in MATLAB, and buttressed by CVODES, a software library that aids with the solving of ordinary differential equations.  Now how will a simulation help further our understanding of cancer?  Well, the claim is that this "model mechanistically interprets context-specific landscapes between driver pathways and cell fates, providing a framework for designing more rational cancer combination therapy.”  So data can be collected from designed situations, a revolutionary advancement.  We can be prepared for an event that has not yet occurred.  Normally a real person has to have cancer for data to be collected, which has lots of constraints.  
# The origin of SPARCED
In 2022, the large-scale pan-cancer model detailed above was published in [*nature communications*](https://www.nature.com/articles/s41467-022-31138-1). What changed? In an environment where there is an abundance of [FAIR](https://www.go-fair.org/fair-principles/) and big omics data sets in literature, the opportunity to build large-scale mechanistic models has increased.  In order for these new models to be re-creatable and/or used as building blocks for whole-cell mechanistic models, there is a need for a standard set of rules (while adhering to FAIR) that detail the appropriate way to build mechanistic models based on canonical biological data.  Enter the SPACRED model, which utilizes easily modifiable text files that are then transformed into [SBML](https://sbml.org/) format prior to model initialization.  This order of operations exponentially decreases the likelihood of bookkeeping errors and ensures additional pathways can be added to the SPARCED model by researchers within its original lab or elsewhere.   
# How to Download SPARCED
We suggest running SPARCED through a Docker Container on your machine.
1. Download [Docker](https://docs.docker.com/get-docker/) and create and account




How is the sparced model laid out <h6> The design is hierarchical.  It is a large model made of many smaller models, one from many.  This allows for incremental improvements, until the model is as comprehensive as it needs to be.  


# How to run the SPARCED model on docker
After all the prerequesites have been complete you are finally ready to run the sparced model.  When that time click [this](https://youtu.be/TpziboQm0qs) link.
