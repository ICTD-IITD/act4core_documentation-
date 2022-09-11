# Community Mapping Team

## Team Members
Ramita (Lead)
Saketh
Om Krishna
Harshita
Aryan
Kirti

## Onboarding Guide
Most of the projects in the team require some basic GIS fundamentals. QGIS and QField are two applications that we use commonly for this end.

It is advisable to start with the following material for the first couple of weeks before you get started on the projects. 

[Community Mapping Overview](https://drive.google.com/file/d/1KmMDia1rryTSPjrsIrAvunyD8fYebAT1/view?usp=sharing) - This slide deck should give a very good overview of things ranging from QGIS Desktop/QGIS Server/QField to various useful datasets and GIS based computations for watersheds. Also will get you to speed to understand what has been done so far.
**Courtesy**: Combined weekly slides by Ramita, Shruti, Sanjali, Dhruv

[GIS fundamentals](https://docs.qgis.org/3.22/en/docs/gentle_gis_introduction/introducing_gis.html) - A gentle introduction to GIS
[QGIS Training Manual](https://docs.qgis.org/3.22/en/docs/training_manual/index.html) - The first 8 chapters give an introduction to handle vectors and rasters.
[QGIS User Guide](https://docs.qgis.org/3.22/en/docs/user_manual/index.html) - More of a reference to go to on a need basis.
[QGIS Server Guide](https://docs.qgis.org/3.22/en/docs/server_manual/index.html) - Chapter 3 to get an understanding of the various ways data could be hosted/fetched from QGIS server.
[PyQGIS cookbook](https://docs.qgis.org/3.22/en/docs/pyqgis_developer_cookbook/index.html) - PyQGIS to automate everything using python without having to use QGIS desktop. A few sections of interest might be:
  * [PyQGIS setup](https://docs.qgis.org/3.22/en/docs/pyqgis_developer_cookbook/intro.html#using-pyqgis-in-standalone-scripts) - setup to run python scripts independently outside qgis desktop's python console
  * [PyQGIS manipulating layers]( https://docs.qgis.org/3.22/en/docs/pyqgis_developer_cookbook/index.html) - Chapter on loading layers, vector and raster manipulation [Chapters 3, 5, 6]
  * [PyQGIS processing guide]( https://docs.qgis.org/3.22/en/docs/user_manual/processing_algs/index.html) - Contains references to various algorithms available for use on vectors and rasters. Useful to see which parameters are needed while running some algorithm on pyqgis.



## Projects

### Catchment and Stream Delineation
The aim of the project is to automate computing different layers like streams and catchment boundaries using pyqgis. This would help simplify the workflow without loading various layers onto QGIS for a particular location.

### Feasibility Assessment App
The idea is to have a simple rule based scoring mechanism for building various water harvesting structures. Once developed, field users should be able to select any point on the app and assess the feasibility of placement of these structures.

### Social Mapping Tool
Field cadre can mark land ownership boundaries at the class/caste level, define socio-economic characteristics of the land owning classes, identify their settlement hamlets as well.

### Village Level Clustering based on ADI, LULC 

**[Project Code](https://github.com/sak-18/village-development-assessment)**

The idea is to leverage various indicators from census, ADI and LULC so as to cluster villages. We could then start deploying or collecting data from villages in these clusters.

## Datasets
You will come across various layers as you work on QGIS ranging from Digital elevation, soil moisture to Land Use Land Cover layers.

A detailed list sources for getting these layers is documented [here](https://docs.google.com/spreadsheets/d/1-ZRog0X46C7bOApfBQLmzejUtlpx245iWaajycAGRz8/edit#gid=0).

Some common layers which you will most likely need for many projects:
* [India Boundary](https://drive.google.com/drive/folders/1WImcF3suHNoAIAcddVp9kFtdchbgSrBQ?usp=sharing)
* [Indian Districts](https://drive.google.com/drive/folders/1qHvNZLPfIrA6AWaT3-jhhEALOHMFGz1_?usp=sharing)  
* [Indian Village Boundaries](https://drive.google.com/file/d/1NoJQwGy4ppWecIeNcERZGufIXEr-WPDD/view?usp=sharing)  


## Slidedeck
Semester-1 2022 - [link](https://drive.google.com/drive/folders/1s2D2MHlOey_m1H4WF_f2Ve-X8bpDrKOx?usp=sharing)

## Backlog
- [x] To document resources spread across spreadsheets, drive links, mail threads 
- [ ] To explore computing drainage lines across India
- [ ] To have a robust way storing and sharing these datasets on catchments or drainage lines once computed (perhaps on google earth catalog)
- [ ] QGIS plugins (to port the automation code for catchment delineation into a plugin)
- [ ] For village boundaries the current [source](https://vlist.in/) is consistent with census 2011, but has missing village boundaries. NASA's SEDAC does provide complete dataset of village boundaries though the boundaries are consistent with 2001 census hence not updated. 