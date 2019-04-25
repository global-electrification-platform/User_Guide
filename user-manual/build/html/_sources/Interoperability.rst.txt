Interoperability
=================================

The GEP is expected to be a part of a continuous data and model 'discovery’ process. This process will – in partnership – discover and develop new data via remote sensing, machine learning, development of new theory and modelling. New data will be compiled, processed in models and new information is expected to be produced during the operation of the GEP. To ensure that this data can easily be integrated to the GEP ecosystem, guidelines for its form and description, as well as ‘handling protocols’ have been developed as presented in the following sections.

Data guidelines
************************************

GEP modules have been designed in such way so as to allow flexibility in integrating electrification related datasets found in other databases and/or platforms as well as analytical outputs from various geospatial tools. Being able to incorporate such datasets or modelling results in the GEP ecosystem is thus an essential part of this initiative.

In order to support the integration process, the GEP team has put together a list of input/output datasets and parameters that are common between several GIS based electrification modelling tools. Each dataset/parameter comes along with suggested standards and metadata describing several characteristics that are important in the integration process. These include type, format, source, author and licence among others.

The list is available `here <https://docs.google.com/spreadsheets/d/1JiV6QT1IBkJR7Q-FntC2zl3aZI2X5IMxrDI9gWupG5M/edit?usp=sharing>`_.

.. note::
    The above list was informed based on the functionalities of the Open Source Spatial
    Electrification Tool (OnSSET), which was used in the development of EISs in GEP 2018 available in **GEP “Explorer”**.

    Replicating EIS (as descried in later sections) using OnSSET 2018 – The GEP version (`link to source code <https://github.com/KTH-dESA/The-GEP>`_) requires that these input/output data guidelines are followed explicitly.

    The GEP team is currently working in collecting feedback from other institutions active in the geospatial electrification modelling (Columbia University, MIT, NRECA, RLI and others) in order to update and expand the current list.

Modelling process guidelines
***********************************

The GEP has been designed upon the core values of transparency, repeatability, and auditability. Therefore, open access of data and modelling processes as well as clear documentation of assumptions on decision parameters is very important. The following paragraphs describe two parts:

    - **Part A.** Pipeline for the development of EISs for a country
    - **Part B.** Configuring & Ingesting EIS results into GEP “Explorer” locally

**Part A.** Pipeline for the development of EISs for a country
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
The pipeline for the development of electrification investment scenarios has been presented in the GEP "Toolbox" section for the case of OnSSET. Although the pipeline is fairly flexible and can be adopted to the modelling framework used, the scenario/results generation shall be developed as per data guidelines presented above.

.. note::

    Changes of the modelling pipeline is possible however, this will also require re-configuration of the GEP “Explorer” as described in the next section. Custom configuration of GEP "Explorer" is possible on local machines. Re-configuration of the online version of the GEP "Explorer" is the output of an annual updating process described below.

Part B. Configuring & Ingesting EIS results into GEP “Explorer” locally
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

The visualization of EIS can be done using any GIS environment. The **GEP "Explorer"** has been developed however, to allow for offline visualization of EIS in the users local working station.
More information on setting the development environment, configuring and ingesting the EIS result data so as to enjoy **GEP "Explorer"** services offline is available `here. <http://devseed.com/gep-docs/>`_

Updating process guidelines (To be updated)
****************************************************
The annual suite of Electrification Investment Scenarios (EIS’s) will include a set of least cost investment scenarios for each target country. The scenarios will be defined by different levels of desired use, the expected costs of technology, and other ‘levers’ etc. These updates will reflect advances in: algorithms and models; improvements in data input; as well as increased scenarios defined by increasingly relevant and available ‘levers’.

In addition, every year an updated version of GEP “Explorer” and GEP “Scenario Generator” will be released. A process will be set up for active updating of these with outreach to partners such that the latest available modelling, data and analysis is both used and compatible with the GEP.  Similarly, each year, advances in standards and updated teaching material will be released.

The first release of the GEP is planned for the *Optimus Community Summer School* in June 2019. Successive releases of the GEP will be made in the last quarter of each year. Calls for input to the GEP will be made and received by August each year.


