The GEP Toolbox
=================================

Overview
************************************

The GEP “Toolbox” provides access to all the ICT ‘widgets’ used in the development of the GEP including tools, methods as well as user manuals and training material. All available in an open an accessible way through various channels. It provides the potential and flexibility needed to fully change the underlying modelling methods and/or generate new models.

Tools and methods
*********************************************************

This version of the GEP uses the `Open Source Spatial Electrification Toolkit (OnSSET) <http://www.onsset.org/>`_. The (OnSSET) source code used to generate the electrification investment scenarios as presented on the GEP "Explorer" is available on `Github <https://github.com/KTH-dESA/The-GEP/tree/The-GEP-Toolbox>`_.

The following steps describe in brief the modelling process followed to generate the scenarios. Many of the steps refer to Malawi which was used as an experimental case study in the development phase. The process can - of course - be replicated for other countries as well.

.. note::
    This section is supported by a open access `peer-reviewed academic publication <https://doi.org/10.3390/en12071395>`_ available online since April 2019.

**Step 1. Collection of necessary data**

The first step in the modelling process requires the collection and preparation of all the necessary datasets and input parameters required to inform the electrification analysis. This include both GIS and non-GIS inputs as described in the section of data guidelines above. All datasets used in GEP are open, with source being provided in metadata. The list is available `here <https://docs.google.com/spreadsheets/d/1JiV6QT1IBkJR7Q-FntC2zl3aZI2X5IMxrDI9gWupG5M/edit?usp=sharing>`__.

An important part of the process requires the construction of population settlements, which is the basis of the electrification analysis in OnSSET. Population settlements are available in the form of raster or vector. The OnSSET model is able to run using either of those, however, the selection defines all next steps in the analysis thus is presented as a separate step. In order to get the most out of the GEP services vector population format is suggested hereafter.

The development team at KTH dESA has developed a methodology for developing population vectors (or population clusters) based on open access, raster population layers. A step-by-step description of the methodology is available `here <https://doi.org/10.3390/en12071395>`__.

.. note::
    The above methodology requires processing in `QGIS <https://www.qgis.org/en/site/>`_ (an open-source GIS software). The KTH team has developed a QGIS plugin that automates the process of population cluster generation. The plugin together with how-to-use instructions are available `here <https://github.com/KTH-dESA>`__.

    The methodology is based on the availability of HRSL population data. In case HRSL data are not available for the country or region of interest a modified version of the methodology can be used. The latter is still under review by the KTH team; please contact the team for further information.

**Step 2. Preparation of OnSSET input data files**

In the second step of the process, the two OnSSET input files are created.

The first file is a comma delimited file (.csv) file. Each row represents a population cluster while each column a characteristic (or attribute) of this cluster. Attributes are extracted from the GIS datasets collected in Step 1. The extraction commands can be executed manually in QGIS. However, the KTH team has created a QGIS plugin in order to automate the process. The plugin is available together with how-to-use instructions `here <https://github.com/KTH-dESA/Cluster-based_extraction_OnSSET>`__.

.. note::
    The number of attributes depends on data availability. For the GEP the input file consists of 24 attribute columns. A sample file of this type is available for Malawi as `"Malawi.csv" <https://github.com/KTH-dESA/The-GEP/tree/The-GEP-Toolbox>`_.

The second file is an excel (.xlsx) file (usually named "Specs") that contains non-GIS input data (e.g. years of analysis, population growth etc.) and calibration parameters of the model.
A listing of those parameters together with their role in the modelling process is available `here <https://docs.google.com/spreadsheets/d/1vMsCQNoe1IDqMgYoGFPZLGO1e0xfxhZiB4_HexwXZ-k/edit#gid=1203867896>`__.

.. note::
    A sample file of this type is available for Malawi as `"specs_mw_one_scenario.xlsx" <https://github.com/KTH-dESA/The-GEP/tree/The-GEP-Toolbox>`_.

**Step 3. Preparation/Calibration of input files**

The third step in the analysis includes the generation (and calibration) of a few additional parameters necessary for the electrification analysis.
These include:

    A. Energy resource indicators (e.g. wind capacity factor, grid suitability)
    B. Population status & projections (Urban Vs Rural population, Electrified Vs non-electrified population (base year))
    C. Definition of demand goals per type of settlement

These functionalities are embedded in the OnSSET code basis. The calibration process takes place in the beginning of a model run and usually happens only once. The code is set to notify the user about the calibration progress via messages in console.

.. note::
    For more information on the calibration process in OnSSET please redirect to the relevant section in the manual available `here <https://onsset-manual.readthedocs.io/en/latest/index.html>`__.

**Step 4. Scenario runs**

The last step of the process requires that the OnSSET model will be set to run a number of predefined EISs. The model is currently configured to generate 144 EISs as a combination of six parameters (hereafter called “levers”)
that include:

    1.	Population growth
    2.	Electricity demand target
    3.	5-year investment plan
    4.	Grid generating cost of electricity
    5.	PV system cost
    6.	Prioritization algorithm

Values and number of options for these levers can be modified via the “specs.xlsx” file. A sample file of this type is available for Malawi as `"specs_mw_144_scenarios.xlsx" <https://github.com/KTH-dESA/The-GEP/tree/The-GEP-Toolbox>`_.

Further description on the functionality of levers is available `here <https://docs.google.com/presentation/d/1OQJi-_24pjgCYNb9N-5hS4T0wx4D2q0UirYkUbzlLLQ/edit#slide=id.g4219fed47f_0_0>`__.

The model yields two types of output files (both .csv) per scenario. The first (full) file contains all the available results and is later on used in the visualization process. The second (light) file contains a summary of the EIS's key parameters (electrification mix, capacity and investment requirements). The list of output parameters along with a brief description is available `here <https://docs.google.com/spreadsheets/d/1vMsCQNoe1IDqMgYoGFPZLGO1e0xfxhZiB4_HexwXZ-k/edit#gid=819349467>`__.

.. note::
    The next version of the GEP will include two additional levers studying the impact of productive uses and diesel price (related to hybrid mini-grids) in the electrification results.

    Changing levers is possible with OnSSET however, this would require further configuration of the model. This of course will require re-configuration of the GEP “Explorer” (described in the next section).

User manual and training material (To be Updated)
*********************************************************

GEP aims to support decision making in various levels (international organizations, government agencies, private sector, other data and modeling groups, individuals etc.) setting up national priorities and identifying critical interventions in the energy field. Training material has been (and still are being) developed and tailored to support the rapid uptake of the GEP “Explorer” and “Scenario generator” applications. It is envisioned that this material will be used in/for:

    * Remote, self-learning (access Video Lectures `here <http://www.patience-is-a-virtue.org/>`__.)

    * In-country training activities (see example `here <http://www.snv.org/update/reaching-sdg7-benin-integrated-energy-planning>`__.)

    * Regional training (such as held at the `Energy Modelling Platform (EMP) <http://www.energymodellingplatform.org/>`_ and the `OpTIMUS Global Summer School on Modelling Tools for Sustainable Development <http://indico.ictp.it/event/8751/>`_

    * Post-graduate curricula (i.g `OpTIMUS Micro-Masters <http://www.patience-is-a-virtue.org/>`_).
