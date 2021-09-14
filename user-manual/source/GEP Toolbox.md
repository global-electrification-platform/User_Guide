# GEP Toolbox

## Overview

The GEP Toolbox provides access to all the ICT 'widgets' used in the development of the GEP including tools, methods as well as user manuals and training material. All available in an open an accessible way through various channels. It provides the potential and flexibility needed to fully change the underlying modelling methods and/or generate new models. 


## Tools and methods

### The Open Source Spatial Electrification Tool (OnSSET)

The current set of results in the GEP were created using a modified version of OnSSET, openly distributed as [gep-onsset](https://github.com/global-electrification-platform/gep-onsset).
In the interests of transparency and collaboration, the modelling process is open for feedback and improvements from other institutions, experts and practitioners. Based on this process, the GEP will be updated annually with improved data and processes, as well as new models.

<div class="note">

<div class="admonition-title"> Note

</div>

A [peer-reviewed academic publication](https://doi.org/10.3390/en12071395) supporting OnSSET modifications for GEP has been developed throughout the duration of the project and is available online since April 2019.

</div>

### Code for developing population clusters

The identification of settlements is the basis of the electrification analysis in many models.
In GEP settlements are represented as vector clusters. KTH dES has developed a methodology for generating such vector clusters based on open access datasets. In the interests of transparency and replicability, KTH dES has also developed the supporting [open source code](https://github.com/babakkhavari/Clustering). In addition, a more detailed description of the methodology is available [here](https://www.nature.com/articles/s41597-021-00897-9?sf245151105=1). 

<div class="note">

<div class="admonition-title"> Note

</div>

The above methodology requires geospatial processing in python.

</div>

### Code for extracting GIS information to vector clusters

Geospatial electrification models are inextricably connected with GIS data. Extracting geospatial information to each vector cluster (see above), is therefore a necessary yet time consuming process.
The extraction commands can be executed manually in QGIS; however, the KTH team has developed an [open source code](https://github.com/babakkhavari/OnSSET_GIS_Extraction_notebook) in order to automate the process.

<div class="note">

<div class="admonition-title"> Note

</div>

In GEP, 26 GIS layers have been used to inform vector attributes as presented [here](https://drive.google.com/file/d/1O3N1vrGJtLEPN4_3_KxJDxqc4cCEo2H9/view?usp=sharing).

</div>


### Data-service and explorer

These refer to the web & data service supporting the GEP. More information is available [here](https://github.com/global-electrification-platform).
 

### User guides & training material

GEP aims to support decision making in various levels. Documentation has been developed 
and tailored to support the rapid uptake of all GEP services, including:

>   - User guides and how-to-use instructions for all tools and methods (refer to each one of them on GEP's [Github page](https://github.com/global-electrification-platform))

>   - Education and Training material on [Google's Open Online Education platform](https://onsset.github.io/teaching_kit/)

## Target Audience

It is envisioned that this material will be used in/for:

>   - Remote, self-learning through video Lectures
>   - In-country training activities (see example [here](http://www.snv.org/update/reaching-sdg7-benin-integrated-energy-planning))
>   - Regional training (such as held at the [Energy Modelling Platform EMP)](http://www.energymodellingplatform.org/) and the [OpTIMUS
>     Global Summer School on Modelling Tools for Sustainable Development](http://indico.ictp.it/event/8751/)
>   - Post-graduate curricula (i.g OpTIMUS Micro-Masters)