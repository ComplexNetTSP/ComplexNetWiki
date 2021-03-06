# Power Grid Datasets

## SciGrid

Territory covered = Europe

Type of network = Transmission grid

Number of nodes = 495

Number of edges = 825

project status = Ongoing

### Description

SciGRID is a project funded by the German Federal Ministry of Education and Research (BMBF). Its intention is to develop methods for the automated generation of models (i.e. maps) of existing electricity grids for research and other purposes. The focus will be on the European transmission grids, but the methods will be applicable more generally. Both the resulting methods and the derived data will be published free of charge under appropriate open source licenses in the course of the project and intends to increase the general availability of network models and their overall quality.

The SciGRID model is written in Python and is mainly based on the "power" relations data available in openstreetmap.org under the Open Database License (ODbL). The "power" relations from OpenStreetMap (OSM) are filtered and exported to relational databases where they are used to build the abstracted transmission network. The relational database approach allows for a flexible and a modular structure of the SciGRID model. 

More information at : http://www.scigrid.de/pages/motivation-and-approach.html

### Documentations

User Guide : http://www.scigrid.de/releases_archive/SciGRID_Userguide_V0.2.pdf

### Publications

http://www.scigrid.de/pages/publications.html

### Downloads

Downloads : http://www.scigrid.de/pages/downloads.html

## GridKit

### Description

GridKit uses spatial and topological analysis to transform map objects from OpenStreetMap into a network model of the electric power system. It has been developed in the context of the SciGRID project at the Next Energy research institute, to investigate the possibility of 'heuristic' analysis to augment the route-based analysis used in SciGRID. This has been implemented as a series of scripts for the PostgreSQL database using the PostGIS spatial extensions.
 
For more information, see https://github.com/bdw/GridKit

### Downloads

Downloads : https://zenodo.org/record/47317#.VvFFr-LhDrc

## The RE-Europe data set

Territory covered = Europe

Type of network =  Transmission grid

Number of nodes = 1494

Number of edges = 2156

project status = ?

### Description

This data set models the continental European electricity system, including demand and renewable energy inflows for the period 2012-2014.

The main features of the data set are:

- High resolution (~50km, 1 hour) and large extent (Mainland Europe, 3 years)
- Technical and economic characteristics of generators from real-world data and best available estimates
- Synthetic wind and solar observations and forecasts from numerical weather prediction models, describing the full spatio-temporal structure of the wind

The transmission system comprises 1494 buses and 2156 lines. For each bus, signals for load, wind and solar production is given for each hour of the three years, with the wind and solar signals based on meteorological weather data.
Further, at hour 00 and 12, forecasts for the solar and wind production are given for the following 91 hours, based on weather data.
All spatially-distributed data is aggregated to the nodal domain by summation/averaging over the area closest to each node.
Wind and solar signals and forecast are given as capacity factors, i.e. production relative to rated power.


### Documentations

See paper at : http://www.powerworld.com/knowledge-base/updated-and-validated-power-flow-model-of-the-main-continental-european-transmission-network

### Downloads

Downloads : https://zenodo.org/record/35177#.VpddovnhBmP



## Power networks/France Project

Territory covered = France

Type of network =  Transmission and distribution

Number of nodes =

Number of edges =

project status = Ongoing

### Description

This project aims at the mapping of the french power grid. Most of the data comes from EDF (main producer), RTE (national transport network and cross border links), and ERDF (main distribution network). 
See interactive map at : http://product.itoworld.com/map/106?lon=2.19496&lat=48.85921&zoom=10

### Documentations

See project Wiki at : http://wiki.openstreetmap.org/wiki/WikiProject_Power_networks/France

### Downloads


## ENTSO-E

Territory covered = Europe

Type of network =  Transmission grid

Number of nodes =

Number of edges =

project status = Ongoing (started in 2014)


### Desriptions

TYNDP 2014 = "Ten-Year Network Development Plan 2014". The TYNDP 2014 explains how ENTSO-E proposes to integrate by 2030 up to 60% of renewable energy, respecting cost-efficiency and security through the planned strengthening of Europe's electricity power grid.
More information at : https://www.entsoe.eu/major-projects/ten-year-network-development-plan/tyndp-2014/Pages/default.aspx

ENTSO-E makes the pan-European power transmission grid datasets used to prepare the TYNDP 2014 available to third parties. The available datasets would assist research and innovation projects in the energy sector in Europe by providing a realistic representation of the European power system; allowing users to validate innovative methods and tools for power system analyses.

In order to ensure data quality and confidentiality requirements (especially reqarding connected customers data), ENTSO-E organises in 2015 a step-wise data publication, starting in June 2015 with a pan-European DC-proxy dataset of the TYNDP 2014.

ENTSO-E plans to further develop the 2030 Vision 1 dataset, especially with respect to voltage control and reactive power data, and possibly generation unit details, subject to confidentiality requirements.

### Documentations

Dynamic Study Model Instruction Manual : https://www.entsoe.eu/Documents/Publications/SOC/Continental_Europe/InitialDynamicModel_Handbook_gen.pdf

### Publications

Dynamic Study Model for the Interconnected Power System of Continental Europe in Different Simulation Tools : https://www.entsoe.eu/Documents/SOC%20documents/Regional_Groups_Continental_Europe/462459.pdf

See list of publications at : https://www.entsoe.eu/publications/position-papers/Pages/default.aspx

### Downloads

The dataset is available in spreadsheets to institutions (universities, companies, IGOs, NGOs, etc.), upon simple request to ENTSO-E.
Use the following form : https://www.entsoe.eu/stum/


## Western US power grid

Territory covered = West part of USA

Type of network =  ??

Number of nodes = 4941

Number of edges = 6594

project status = Ended

### Descriptions

Undirected and unweighted network representing the topology of the Western States Power Grid of the United States.

Problem : We lack information about what exactly do the nodes and edges represent. Furthermore, there is no information about production sites, line capacities and so on.

### Publications

Collective dynamics of ‘small-world’ networks : http://www.nature.com.gate6.inist.fr/nature/journal/v393/n6684/full/393440a0.html

### Downloads

http://nexus.igraph.org/api/dataset_info?id=15&format=html


## Data.gouv.fr

* [Donnée ERDF](https://www.etalab.gouv.fr/erdf-poursuit-son-avancee-dans-lopen-data-au-cote-detalab)

## pecanstreet Solar production + Energy comsuption 

* [Pecanstreet](https://dataport.pecanstreet.org/)