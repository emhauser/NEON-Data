###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.
DATA PRODUCT INFORMATION
------------------------
ID: NEON.DOM.SITE.DP1.10026.001
Name: Plant foliar traits
Description: Traits of sun-lit canopy plants reported at the level of the individual (woody plants) or community (herbaceous plants).
NEON Science Team Supplier: Terrestrial Observation System
Abstract: This data product contains the quality-controlled, native sampling resolution data from NEON's measurement of foliar traits in sun lit, georeferenced vegetation samples. Trait measurements include leaf mass per area, leaf water content, chlorophyll, carbon and nitrogen concentrations and stable isotopes, major and minor elements, and lignin. Whenever possible, foliar data are collected in conjunction with overflights of the NEON Airborne Observation Platform (AOP), and starting in 2020 polygon shapefiles are provided to link sampled crowns to airborne imagery. For additional details, see the user guide, protocols, and science design listed in the Documentation section below. Queries for this data product will return field collection data, physical and chemical measurements, and crown polygons (where available) on a per sample basis. Several items are available in the expanded data package, including summary tables of external lab precision and accuracy as well as information on woody sample geolocation.
Latency:
The expected time from data and/or sample collection in the field to data publication is as follows, for each of the data tables (in days) in the downloaded data package. See the Data Product User Guide for more information.
bgc\_CNiso\_externalSummary:  30
cfc_carbonNitrogen:  270
cfc_chemistrySubsampling:  90
cfc_chlorophyll:  120
cfc_chlorophyllParameters:  30
cfc_chlorophyllSummary:  30
cfc_elements:  180
cfc_elementsSummary:  30
cfc_fieldData:  90
cfc_lignin:  180
cfc_LMA:  90
cfc_shapefile: 90
lig_externalSummary:  30
vst_mappingandtagging: 120
Brief Design Description: For sites with predominantly forest/shrubland cover, spatial collection methods differed during early operations (2016???2018) compared to 2019 and onward. The earlier method involved sampling the top three dominant species present in each of 14 pre???assigned plots, 4 Tower and 10 Distributed. However, with input from the community, the design shifted away from plots and towards a site???based approach focused on sampling the full spectrum of canopy biodiversity present at the site. Many of the individuals sampled are monitored in the Vegetation Structure (VST) protocol, and all are georeferenced, either using stem offsets (prior to 2020 as well as smaller individuals) or polygon shapefiles of sampled crowns mapped on top of recent AOP spectrometer data while in the field (2020 and onward for larger individuals).
For grassland sites, the design has remained consistent. Foliage is sampled from 20 plots; all aboveground material in one or two (depending on plot size), randomly selected  0.1 X 2 m clip strips is harvested and homogenized, yielding 20-24 samples per bout. Traits are measured on species mixtures that represent community composition of the clip strip. In sites with both woody and herbaceous cover, a combination of the two sampling approaches is employed.
Foliar sampling occurs once every five years per site during the period of historic peak greenness. Whenever possible, sampling also occurs within two weeks of the AOP overflight and aopCollectDate for each sample is included in the data. Chlorophyll subsamples are immediately frozen after collection, and additional processing of samples, including scans for leaf mass per area and initiation of sample drying for leaf water content and chemical analyses, occurs within 1-5 days of collection. During the same year that foliar traits are measured, other biogeochemical pools and fluxes are as well (e.g., soil chemistry, DP1.10086.001; litter chemistry, DP1.10033.001; root biomass and chemistry, DP1.10067.001) with coincident data at a subset of plots.
Brief Study Area Description: Foliar sampling is conducted at all NEON terrestrial sites.
Sensor(s): 
Keywords: boron (B), calcium (Ca), zinc (Zn), carbon (C), iron (Fe), foliage, sulfur (S), specific leaf area, manganese (Mn), chlorophyll, leaves, canopy, cellulose, foliar, potassium (K), phosphorous (P), leaf mass per area, carotenoids, magnesium (Mg), lignin, copper (Cu), plants, nitrogen (N)
Domain: D01
DATA PACKAGE CONTENTS
---------------------
This folder contains the following documentation files:
This data product contains up to 14 data tables:
- Term descriptions, data types, and units: NEON.D01.HARV.DP1.10026.001.variables.20211222T024324Z.csv
cfc_LMA - Leaf mass per area measurement of foliar samples
cfc_lignin - External lab analysis of lignin concentrations in foliage
cfc_chlorophyll - External lab analysis of foliar chlorophyll concentrations
cfc_elements - External lab analysis of major, minor, and trace element concentrations in foliage
cfc_chlorophyllParameters - External lab parameters used in foliar chlorophyll measurements
cfc_fieldData - Field collection of foliar samples
cfc_carbonNitrogen - External lab analysis of carbon and nitrogen concentrations and stable isotopes in foliage
lig_externalSummary - Long-term uncertainty values for lignin analysis in plant tissue
cfc_shapefile - Metadata for shapefiles that contain crown polygons
vst_mappingandtagging - Mapping, identifying and tagging of individual stems for remeasurement
ISSUE LOG
----------
This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10026.001.
Issue Date: 2021-01-06
Issue: Safety measures to protect personnel during the COVID-19 pandemic resulted in reduced or eliminated sampling activities for extended periods at NEON sites. Data availability may be reduced during this time.
       Date Range: 2020-03-23 to 2021-06-01
       Location(s) Affected: All
Resolution Date: 
Resolution: 
Issue Date: 2021-10-29
Issue: Due to the logistics of the airborne and field sampling schedules, as well as sporadic issues with protocol implementation, foliar samples are not always collected within two weeks of the AOP overflight. Some traits (e.g., pigments, water content) are known to change over the course of the growing season, thus it is helpful for data users to know when samples were collected relative to the remote sensing data in order to decide how to apply foliar data for modeling or validation studies.
       Date Range: 2016-01-01 to 2021-11-08
       Location(s) Affected: All terrestrial sites sampled during this period.
Resolution Date: 
Resolution: In order to communicate the temporal coupling of the two data streams, a new field called 'aopCollectDate' was added to the cfc_fieldData table. Is it not currently possible to add this information for foliar samples associated with field spectral measurements, but this is planned for the future.
Issue Date: 2021-12-09
Issue: Prior to the 2022 data release, publication of species identifications were obfuscated to a higher taxonomic rank when the taxon was found to be listed as threatened, endangered, or sensitive at the state level where the observation was recorded. Obfuscating state-listed taxa has created challenges for data users studying biodiversity.
       Date Range: 2012-01-01 to 2021-12-31
       Location(s) Affected: All
Resolution Date: 2021-12-31
Resolution: The state-level obfuscation routine was removed from the data publication process at all locations excluding sites located in D01 and D20. Data have been reprocessed to remove the obfuscation of state-listed taxa. Federally listed threatened and endangered or sensitive species remain obfuscated at all sites and sensitive species remain redacted at National Park sites.
Issue Date: 2020-12-01
Issue: Due to a miscommunication, samples analyzed for carbon (C) and nitrogen (N) concentrations and stable isotopes were not re-dried prior to weighing and analysis at the external lab. While all NEON foliage samples are dried at 65C in the domain labs, they are sometimes then stored in paper bags or coin envelopes for weeks or even months before being ground, transferred to vials, and shipped. During this time they may accumulate moisture, especially in humid areas. Subsequent testing revealed that %C data are likely underestimated by 1.5-2.5% due to this lack of re-drying prior to analysis. As vegetation samples tend to have high %C (20% - 55%), this bias may have only minor impacts on many analyses, but is something for end users to keep in mind. For the other parameters (%N, C:N, d15N, d13C), testing suggests there were no detectable differences between re-dried samples and originals.
       Date Range: 2016-01-01 to 2020-09-08
       Location(s) Affected: All sites with foliar chemistry measurements in this date range, with the exception of GUAN and PUUM whose tissues were re-dried for permitting/quarantine reasons.
Resolution Date: 2020-11-10
Resolution: Affected data have been flagged with dataQF = dryingProtocolError in the `cfc_carbonNitrogen` table. For sample analysis dates starting in November 2020, all carbon-nitrogen samples are re-dried at 65C prior to analysis to drive out any residual moisture and improve data accuracy for % C. Samples collected in 2020 may have been analyzed before or after the change; check dataQF to determine which individual samples are affected.
Issue Date: 2019-10-15
Issue: Possible data quality issues with major, minor, and trace element concentrations (`cfc_elements` table) measured in sunlit plant foliage tissue collected in 2017 and 2018. Data removed on 2019-10-14 due to quality issues with external lab analyses.
       Date Range: 2017-01-01 to 2018-12-31
       Location(s) Affected: HARV, SCBI, DSNY, GUAN, STEI, KONZ, UKFS, ORNL, MLBS, TALL, LENO, STER, OAES, MOAB, JORN, SOAP, TOOL, DEJU
Resolution Date: 2020-10-29
Resolution: Samples re-analyzed using material from the NEON Biorepository and new data loaded 2020-10-29.
Issue Date: 2020-10-02
Issue: Until October 2020, foliar chemistry and stable isotopes were published as separate data products.
       Date Range: 2016-01-01 to 2020-10-06
       Location(s) Affected: All terrestrial sites sampled during this period.
Resolution Date: 2020-10-06
Resolution: In October 2020, data tables for chemistry and isotopes were bundled together in a single data product for improved usability. This applies to all existing and future data.
Issue Date: 2020-10-08
Issue: Prior to the 2020 field season, there was no mechanism to indicate when and why a scheduled sampling event may have been missed.
       Date Range: 2016-01-01 to 2019-12-31
       Location(s) Affected: CLBJ, DCFS, DSNY, KONA, KONZ, MOAB, OAES, SJER, STER, TOOL, WOOD
Resolution Date: 2020-01-01
Resolution: Starting in the 2020 field season, NEON added the field samplingImpractical to the `cfc_fieldData` table of this data product to assist users in understanding when data for this product are temporarily missing versus permanently unavailable. If field collection of an herbaceous clip strip from an assigned foliar sampling plot or subplot was not possible, samplingImpractical is populated with a value other than 'OK' (e.g., 'location flooded' or 'logistical') and only minimal metadata are recorded. Note that this is only relevant for herbaceous-dominated sites (grasslands). For sites dominated by woody individuals (forests/shrublands), this field is not used since there is no assigned list of plots/subplots.
Issue Date: 2020-10-02
Issue: In forested and shrubland sites, the original protocol was to sample a fixed number of woody individuals (n = 3) from an assigned list of plots (n = 14). In consultation with the Foliar Sampling TWG and other researchers, we decided that the focus should be on capturing the breadth of canopy species diversity across that site, and therefore the sampling strategy needed to shift.
       Date Range: 2016-01-01 to 2018-12-31
       Location(s) Affected: DEJU, GRSM, GUAN, HARV, JORN, LENO, MLBS, ORNL, SCBI, SERC, SOAP, STEI, TALL, UKFS
Resolution Date: 2019-01-01
Resolution: From 2019 and onward, forest and shrubland sites sample according to a target taxa list, which contains all species present in the canopy (more diverse sites have longer lists and therefore more samples). The most common taxa are sampled with replication, with individuals spread out to capture site gradients, and rare species are sampled where possible. See the Protocol and Data Product User Guide for more details.
ADDITIONAL INFORMATION
----------------------
Queries for this data product will return data collected during the date range specified. Each foliage sample has a unique identifier (sampleID) that is expected to appear once in the `cfc_fieldData` table. A record from `cfc_fieldData` is then expected to appear once in `cfc_LMA` and in `cfc_chemistrySubsampling`, with several subsamples created. Each record from `cfc_chemistrySubsampling` is expected to appear one to several times (if analytical replicates were conducted) in `cfc_chlorophyll`, `cfc_carbonNitrogen`, `cfc_elements` and `cfc_lignin`. There should only be one instance per sampleID x analyticalRepNumber (x co2Trapped entry in the carbon-nitrogen table), but duplicates may exist where protocol and/or data entry aberrations have occurred. Users should check data carefully for anomalies before analyzing data.
NEON DATA POLICY AND CITATION GUIDELINES
----------------------------------------
A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10026.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.
DATA QUALITY AND VERSIONING
---------------------------
NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI.
To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.
