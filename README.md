# Welcome
The purpose of this page is to share the basic knowledge required to operate the SPARCED model. We do not intend for this page to be a comprehensive guide to the SPARCED model. Instead, we hope this will serve as a self-contained roadmap for future Clemson University Creative Inquiry (C.I.) students to familiarize themselves with the model efficiently and begin to run SPARCED simulations independently.
# Layout
> - Pan-Cancer Model
> - Origin of SPARCED Model
> - SPARCED Model Design
> - Running SPARCED on Docker
> - Running SPARCED on Palmetto
> - Role of a C.I. Student
> - Current Tasks
#  Pan-Cancer Model <h6> 
To entirely understand what the SPARCED model is, it is best learn what it came from.  This would be the PAN-cancer model.  The official paper can be found [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5886578/).  This is a mechanistic model of Cancer in a MCF10A cell, which is a non-tumorigenic epithelial cell line.  The model is an "integrated system of ordinary differential equations"  which was coded in MATLAB, and buttressed by CVODES, a software library that aids with the solving of ordinary differential equations.  Now how will a simulation help further our understanding of cancer?  Well, the claim is that this "model mechanistically interprets context-specific landscapes between driver pathways and cell fates, providing a framework for designing more rational cancer combination therapy.”  So data can be collected from designed situations, a revolutionary advancement.  We can be prepared for an event that has not yet occurred.  Normally a real person has to have cancer for data to be collected, which has lots of constraints.  
# Origin of SPARCED Model
In 2022, the large-scale pan-cancer model detailed above was published in [*nature communications*](https://www.nature.com/articles/s41467-022-31138-1). What changed? In an environment where there is an abundance of [FAIR](https://www.go-fair.org/fair-principles/) and big omics data sets in literature, the opportunity to build large-scale mechanistic models has increased.  In order for these new models to be re-creatable and/or used as building blocks for whole-cell mechanistic models, there is a need for a standard set of rules (while adhering to FAIR) that detail the appropriate way to build mechanistic models based on canonical biological data.  Enter the SPACRED model, which utilizes easily modifiable text files that are then transformed into [SBML](https://sbml.org/) format prior to model initialization.  This order of operations exponentially decreases the likelihood of bookkeeping errors and ensures additional pathways can be added to the SPARCED model by researchers within its original lab or elsewhere.   


# SPARCED Model Design 
The design is hierarchical.  It is a large model made of many smaller models, one from many.  This allows for incremental improvements, until the model is as comprehensive as it needs to be.  Part of your job will be to find, assess, and add new bits on to the model.  How this is done will be touched on later.  The model is made with what is called scientific computing.  This approach is done by implementing mathmatical models, such as ordinary differential equations, on a computer.  This nuanced method allows for data to be generated quickly and accurately.  More about the sparced model's scientific computing can be found [here](https://docs.google.com/presentation/d/1-BdB6zB-agxxQZO4oOsBik_GF07Yeu2AvfM71NwmMIA/edit#slide=id.g2850f5059d4_0_10).


# Running the SPARCED Model on Docker
The SPARCED model can be run through Docker.  First go to the Docker website, make an account and download Docker.  Then once that is done the sparced model can be run.  [This link](https://youtu.be/TpziboQm0qs) will walk you through exactly how to do that.  To learn more about Docker go [here](https://www.Docker.com/resources/what-container/).

# Running the SPARCED Model on Palmetto
Larger more comprehenisve data sets require more computing power to generate in a timely manner.  If buying a supercomputer is not something that can be easily accomplished, Palmetto can be used. [This link](https://docs.google.com/presentation/d/1Doqqxc7U7tEDwjnZbUdJFkDByoTOyPUZQHn0qXMnG3g/edit#slide=id.p) will walk you through exactly how to do that.  More about what Palmetto is can be found [here](https://docs.rcd.clemson.edu/Palmetto/about/).

# Role of a C.I. Student
Intially what must be done is everything outlined thus far.  Then new models that can be integrated into the model must be found.  First a model must be found, then its paper read.  It must be assesed to see if it is reliable, and if it is, it must be decided if it will it be easy to integrate into the SPARCED model.  This is a slow process because, as you will find out, reading papers take a good deal of time.  

# Currently: adding a new pathway into the model-- TGF-Beta Pathway
![1701893175083-3eba7d6c-eae6-457b-a32d-df7bae9af59e_1](https://github.com/Chubbysoap/Sparced-intro/assets/18647080/adc39f43-9f20-484a-818c-8339eb2ece67)

