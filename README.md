# madagascar_malaria_prevalence_2021

Code used to analyze malaria prevalence data from 2013-2017 field studies. For descriptions of the field studies, see:

1. Golden CD, Anjaranirina EJG, Fernald LCH, Hartl DL, Kremen C, Milner DA Jr, et al. Cohort Profile: The Madagascar Health and Environmental Research (MAHERY) study in north-eastern Madagascar. Int J Epidemiol. 2017;46:1747–8d.

2. Golden CD, Borgerson C, Rice BL, Allen LH, Anjaranirina EJG, Barrett CB, et al. Cohort Description of the Madagascar Health and Environmental Research-Antongil (MAHERY-Antongil) Study in Madagascar. Front Nutr. 2019;6:109.

3. Golden CD, Rice BL, Randriamady HJ, Vonona AM, Randrianasolo JF, Tafangy AN, et al. Study Protocol: A Cross-Sectional Examination of Socio-Demographic and Ecological Determinants of Nutrition and Disease Across Madagascar. Front Public Health. 2020;8:500.

In addition to the code used in data cleaning and analysis, this repository will contain a the csv file with the malaria infection outcome line data used in analysis

Benjamin L. Rice
2021

**Additional File 1** Additional File 1.csv contains the malaria rapid diagnostic test outcome data as a line list

Description of column names:
`unique_ind_id` : Unique numeric identifier for each sampled individual
`region_id` : Numeric identifier for each study region
`region_name` : Identifier for each study region (includes region code, e.g., `NE` for Northeast Region) and name of nearest urban center for which the region is named
`site_code` : Identifier for each study site (includes region code, e.g., `NE` for Northeast Region)
`site_id` : Numeric identifier for each study site
`hh_id` : Numeric identifier for each sampled household
`ageyears` : Age in years for the individual
`sex` : Male or female
`time_point_code` : Numeric code for the seasonal time point of sampling
`time_point_date` : The time period over which sampling for that time point occurred
`sample_date` : Day of sampling (day RDT was performed) for the individual
`rdt_result` : Negative (0) or positive (1) result for malaria RDT (see methods)

**Supplementary Table 1** Supplementary Table 1.csv contains sampling dates and malaria prevalence data by site and household

Description of column names:
`site_id` : Numeric identifier for each study site
`site_code` : Identifier for each study site (includes region code, e.g., `NE` for Northeast Region)
`time_point_code` : Numeric code for the seasonal time point of sampling
`site_tp` : A combination of the `site_id` and `time_point_code`
`time_point_date` : The time period over which sampling for that time point occurred
`sample_date_start` : First day of sampling for that site for that time point
`sample_date_end` : Last day of sampling for that site for that time point
`region_id` : Numeric identifier for each study region
`region_name` : Includes the name of the urban center nearest the rural study communities
`region_peak_mo` : The estimated month of peak malaria incidence for that region per [Arambepola et al 2020](https://pubmed.ncbi.nlm.nih.gov/33093622/)
`n_site` : Number of individuals sampled
`n_rdt_pos_site` : Number of RDT positive individuals observed
`prev_site` : Proportion of sampled individuals that were RDT positive
`prev.2_10` : Proportion of sampled children aged 2-10 years that were RDT positive
`n_hh_site` : Number of households sampled
`prev_hh` : Proportion of sampled households with 1+ RDT positive individuals
`adj_cons_area`: Nearest conservation priority or officially protected area(s) for each study site
`dist_to_cons_area` : Approximate distance in km of study site to forest edge or edge of conservation area
`district` : Districts are second-level administrative divisions in Madagascar
`commune` : Communes are third-level administrative divisions in Madagascar
