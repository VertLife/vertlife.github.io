---
layout: default
title: Traits
weight: 4
incognito: true
---

{::options parse_block_html="true" /}

<!-- [**Back to main**](http://vertlife.org/) -->

# TetrapodTraits Database  

**Abstract**: Tetrapods (amphibian, reptiles, birds and mammals) are model systems for global biodiversity science, but continuing data gaps, limited data standardisation, and ongoing flux in taxonomic nomenclature constrain integrative research on this group and potentially cause biassed inference. We combined and harmonised taxonomic, spatial, phylogenetic, and attribute data with phylogeny-based multiple imputation to provide a comprehensive data resource (TetrapodTraits 1.0.0) that includes values, predictions, and sources for body size, activity time, micro- and macrohabitat, ecosystem, threat status, biogeography, insularity, environmental preferences and human influence, for all 33,281 tetrapod species covered in recent fully sampled phylogenies. We assess gaps and biases across taxa and space, finding that shared data missing in attribute values increased with taxon-level completeness and richness across clades. Prediction of missing attribute values using multiple imputation revealed substantial changes in estimated macroecological patterns. These results highlight biases incurred by non-random missingness and strategies to best address them. While there is an obvious need for further data collection and updates, our phylogeny-informed database of tetrapod traits can support a more comprehensive representation of tetrapod species and their attributes in ecology, evolution, and conservation research. 

**Additional Information:** This work is also available at [10.5281/zenodo.10530618](https://zenodo.org/records/10530618).

**Version 1.0.0** (19 April 2024). TetrapodTraits, the full phylogenetically coherent database we developed, is being made publicly available to support a range of research applications in ecology, evolution, and conservation and to help minimise the impacts of biassed data in this model system. The database includes 24 species-level attributes linked to their respective sources across 33,281 tetrapod species. Specific fields clearly label data sources and imputations in the TetrapodTraits, while additional tables record the 10K values per missing entry per species. 

1. Taxonomy – includes 8 attributes that inform scientific names and respective higher-level taxonomic ranks, authority name, and year of species description. Field names: Scientific.Name, Genus, Family, Suborder, Order, Class, Authority, and YearOfDescription. 
2. Phylogenetic tree – includes 2 attributes that notify which fully-sampled phylogeny contains the species, along with whether the species placement was imputed or not in the phylogeny. Field names: TreeTaxon, TreeImputed. 
3. Body size – includes 7 attributes that inform length, mass, and data sources on species sizes, and details on the imputation of species length or mass. Field names: BodyLength_mm, LengthMeasure, ImputedLength, SourceBodyLength, BodyMass_g, ImputedMass, SourceBodyMass. 
4. Activity time – includes 5 attributes that describe period of activity (e.g., diurnal, fossorial) as dummy (binary) variables, data sources, details on the imputation of species activity time, and a nocturnality score. Field names: Diu, Noc, ImputedActTime, SourceActTime, Nocturnality. 
5. Microhabitat – includes 8 attributes covering habitat use (e.g., fossorial, terrestrial, aquatic, arboreal, aerial) as dummy (binary) variables, data sources, details on the imputation of microhabitat, and a verticality score. Field names: Fos, Ter, Aqu, Arb, Aer, ImputedHabitat, SourceHabitat, Verticality. 
6. Macrohabitat – includes 19 attributes that reflect major habitat types according to the IUCN classification, the sum of major habitats, data source, and details on the imputation of macrohabitat. Field names: MajorHabitat_1 to MajorHabitat_10, MajorHabitat_12 to MajorHabitat_17, MajorHabitatSum, ImputedMajorHabitat, SourceMajorHabitat. MajorHabitat_11, representing the marine deep ocean floor (unoccupied by any species in our database), is not included here. 
7. Ecosystem – includes 6 attributes covering species ecosystem (e.g., terrestrial, freshwater, marine) as dummy (binary) variables, the sum of ecosystem types, data sources, and details on the imputation of ecosystem. Field names: EcoTer, EcoFresh, EcoMar, EcosystemSum, ImputedEcosystem, SourceEcosystem. 
8. Threat status – includes 3 attributes that inform the assessed threat statuses according to IUCN red list and related literature. Field names: IUCN_Binomial, AssessedStatus, SourceStatus. 
9. RangeSize – the number of 110×110 grid cells covered by the species range map. Data derived from [MOL](https://mol.org/). 
10. Latitude – coordinate centroid of the species range map. 
11. Longitude – coordinate centroid of the species range map. 
12. Biogeography – includes 8 attributes that present the proportion of species range within each WWF biogeographical realm. Field names: Afrotropic, Australasia, IndoMalay, Nearctic, Neotropic, Oceania, Palearctic, Antarctic. 
13. Insularity – includes 2 attributes that notify if a species is insular endemic (binary, 1 = yes, 0 = no), followed by the respective data source. Field names: Insularity, SourceInsularity. 
14. AnnuMeanTemp – Average within-range annual mean temperature (Celsius degree). Data derived from [CHELSA v. 1.2](https://chelsa-climate.org/). 
15. AnnuPrecip – Average within-range annual precipitation (mm). Data derived from [CHELSA v. 1.2](https://chelsa-climate.org/).
16. TempSeasonality –  Average within-range temperature seasonality (Standard deviation × 100). Data derived from [CHELSA v. 1.2](https://chelsa-climate.org/). 
17. PrecipSeasonality –  Average within-range precipitation seasonality (Coefficient of Variation). Data derived from [CHELSA v. 1.2](https://chelsa-climate.org/). 
18. Elevation – Average within-range elevation (metres). Data derived from topographic layers in EarthEnv. 
19. ETA50K – Average within-range estimated time to travel to cities with a population >50K in the year 2015. Data from [Nelson et al. (2019)](https://doi.org/10.1038/s41597-019-0265-5). 
20. HumanDensity – Average within-range human population density in 2017. Data derived from [HYDE v. 3.2](https://www.pbl.nl/en/image/links/hyde). 
21. PropUrbanArea – Proportion of species range map covered by built-up area, such as towns, cities, etc. at year 2017. Data derived from [HYDE v. 3.2](https://www.pbl.nl/en/image/links/hyde). 
22. PropCroplandArea – Proportion of species range map covered by cropland area, identical to FAO's category 'Arable land and permanent crops' at year 2017. Data derived from [HYDE v. 3.2](https://www.pbl.nl/en/image/links/hyde). 
23. PropPastureArea – Proportion of species range map covered by cropland, defined as Grazing land with an aridity index > 0.5, assumed to be more intensively managed (converted in climate models) at year 2017. Data derived from [HYDE v. 3.2](https://www.pbl.nl/en/image/links/hyde). 
24. PropRangelandArea – Proportion of species range map covered by rangeland, defined as Grazing land with an aridity index < 0.5, assumed to be less or not managed (not converted in climate models) at year 2017.  Data derived from [HYDE v. 3.2](https://www.pbl.nl/en/image/links/hyde). 


## File descriptions: 

* **ImputedSets.zip** – the phylogenetic multiple imputation framework applied to the TetrapodTraits database produced 10,000 imputed values per missing data entry (= 100 phylogenetic trees x 10 validation-folds x 10 multiple imputations). These imputations were specifically developed for four fundamental natural history traits: Body length, Body mass, Activity time, and Microhabitat. To facilitate the evaluation of each imputed value in a user-friendly format, we offer 10,000 tables containing both observed and imputed data for the 33,281 species in the TetrapodTraits database. Each table encompasses information about the four targeted natural history traits, along with designated fields (e.g., ImputedMass) that clearly indicate whether the trait value provided (e.g., BodyMass_g) corresponds to observed (e.g., ImputedMass = 0) or imputed (e.g., ImputedMass = 1) data. Given that the complete set of 10,000 tables necessitates nearly 17GB of storage space, we have organized sets of 1,000 tables into separate zip files to streamline the download process. 

    * ImputedSets_1K.zip, imputations for trees 1 to 10. 
    * ImputedSets_2K.zip, imputations for trees 11 to 20. 
    * ImputedSets_3K.zip, imputations for trees 21 to 30. 
    * ImputedSets_4K.zip, imputations for trees 31 to 40. 
    * ImputedSets_5K.zip, imputations for trees 41 to 50. 
    * ImputedSets_6K.zip, imputations for trees 51 to 60. 
    * ImputedSets_7K.zip, imputations for trees 61 to 70. 
    * ImputedSets_8K.zip, imputations for trees 71 to 80. 
    * ImputedSets_9K.zip, imputations for trees 81 to 90. 
    * ImputedSets_10K.zip, imputations for trees 91 to 100. 

* **TetrapodTraits_1.0.0.csv** –  the complete TetrapodTraits database, with missing data entries in natural history traits (body length, body mass, activity time, and microhabitat) replaced by the average across the 10K imputed values obtained through phylogenetic multiple imputation. Please note that imputed microhabitat (attribute fields: Fos, Ter, Aqu, Arb, Aer) and imputed activity time (attribute fields: Diu, Noc) are continuous variables within the 0-1 range interval. At the user's discretion, the types of microhabitat and activity time can be transformed into binary variables using a predefined threshold (e.g., 0.50), although we recommend utilizing the original imputed values. 
* **Tetrapod_360.csv** – spatial intersections of the 110 x 110 km quadrats (gridcells_110km.zip) with species geographic range maps from https://mol.org. 

**External files:** The R-code used for data analysis is available at [10.5281/zenodo.10582070](https://zenodo.org/records/10976274). The grid cell shapefiles at 110 km of spatial resolution required to mapping of species included in the Tetrapod_360.csv is available through the file Shapefile.zip ([here](https://zenodo.org/records/10976274)). 

**Funding:** We gratefully acknowledge support from São Paulo Research Foundation (FAPESP, grants #2021/11840-6, #2022/12231-6, #2016/25358-3, #2020/12558-0, #2022/15247-0); Coordenação de Aperfeiçoamento de Pessoal de Nível Superior (CAPES);  Conselho Nacional de Desenvolvimento Científico (CNPq, research grants #311504/2020-5 and #302834/2020-6); United States National Science Foundation (NSF, grants DEB-1441719, DEB-1441652, DEB-1441737, and DEB-1441719); NASA (grants 80NSSC17K0282 and 80NSSC18K0435); and the E.O. Wilson Biodiversity Foundation. 

**Reference:** Moura, M.R., Ceron, K., Guedes, J.J.M., Chen-Zhao, R., Sica, Y.V., Hart, J., Dorman, W., Gonzalez-del-Pliego, P., Ranipeta, A., Catenazzi, A.., Werneck, F.P., Toledo, L.F., Upham, N.S., Tonini, J.F.R., Colston, T.J., Guralnick, R., Bowie, R.C.K., Pyron, R.A., Jetz, W. A phylogeny-informed characterisation of global tetrapod traits addresses data gaps and biases. BioRXiv, 2024, doi: [10.1101/2023.03.04.531098v3](https://www.biorxiv.org/content/10.1101/2023.03.04.531098v3)

 