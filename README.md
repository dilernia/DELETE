---
execute:
  echo: false
  message: false
  output: true
  warning: false
title: Michigan PFAS Data
toc-title: Table of contents
---

## Description

From the state of Michigan's website:

*PFAS are a large group of man-made chemicals that include
perfluorooctanoic acid (PFOA) and perfluorooctanesulfonic acid (PFOS).
PFAS have been used globally during the past century in manufacturing,
firefighting and thousands of common household and other consumer
products. These chemicals are persistent in the environment and in the
human body -- meaning they don't break down and they can accumulate over
time. In recent years, experts have become increasingly concerned by the
potential effects of high concentrations of PFAS on human health.*

PFAS contamination in West Michigan has unfortunately made
[headlines](https://www.wzzm13.com/article/news/local/judge-approves-54m-settlement-kent-co-residents-wolverine-3m-pfas-case/69-091ea42c-125a-4341-8ea0-238fdac4d06e),
reminiscent of other environmental advocacy efforts like that of
renowned whistleblower [Erin
Brockovich](https://en.wikipedia.org/wiki/Erin_Brockovich).

There are multiple PFAS-related data sets available from the state of
Michigan contained in a single zipped file on
[GitHub](https://github.com/dilernia/STA418-518/blob/main/Data/pfas_data.zip)
<https://github.com/dilernia/STA418-518/blob/main/Data/pfas_data.zip>:

1.  **Surface water sampling data**; PFAS concentrations in surface
    water samples 🏞🐟

2.  **Public water supply sampling data**; PFAS concentrations in
    municipal drinking water samples 💧🫗

3.  **PFAS sites data** ; PFAS contamination or investigation sites of
    interest ☢️🏭

The original data dictionary for the full surface water data is
available at
<https://gis-egle.hub.arcgis.com/datasets/egle::pfas-surface-water-sampling/about>.

A non-comprehensive laboratory PFAS analyte list (showing for example
that PFTeDA is Perfluorotetradecanoic acid) for analyzing data collected
by Michigan's Departments of Environment, Great Lakes, and Energy
(EGLE), Health and Human Services (HHS), Agriculture and Rural
Development, and Natural Resources can be found
[here](https://www.michigan.gov/pfasresponse/-/media/Project/Websites/PFAS-Response/Sampling-Guidance/Minimum-Laboratory-Analyte-List.pdf?rev=a35aba56ec5a4922b986f01e25c1a19d&hash=04E6F164AA5F5CD29B83B39983341345):
<https://www.michigan.gov/pfasresponse/-/media/Project/Websites/PFAS-Response/Sampling-Guidance/Minimum-Laboratory-Analyte-List.pdf?rev=a35aba56ec5a4922b986f01e25c1a19d&hash=04E6F164AA5F5CD29B83B39983341345>.

## Source

Data was obtained from the state of Michigan website
<https://gis-egle.hub.arcgis.com/search?q=pfasgis>.

## Data Dictionary

### Surface water sampling data

:::: cell
::: cell-output-display
  --------------------------------------------------------------------------------------
  Variable                 Description
  ------------------------ -------------------------------------------------------------
  geoid                    geographic region ID with the first 2 digits being the state
                           Federal Information Processing Standard (FIPS) code and the
                           last 3 digits the county FIPS code

  longitude                The longitude coordinate for the sampling location

  latitude                 The latitude coordinate for the sampling location

  lab_sample_id            The sample ID provided by the analytical laboratory

  site_code                The sampling location name

  coc_sample_id            The sample ID listed on chain of custody provided to the
                           analytical laboratory

  sample_type              An expanded description of what type of sample was collected

  lab_name                 The name of the analytical laboratory used for analysis of
                           the sample

  lab_job_name             The analytical laboratories job/work order name

  collection_date          The date that the sample was collected

  analysis_method          The analysis method used by the analytical laboratory to
                           analyze the sample

  dilution_factor          The dilution factor used by the analytical laboratory during
                           sample preparation

  analysis_date            The date that the analysis was conducted by the analytical
                           laboratory

  duplicate                A description of what type of sample was collected

  watershed                The watershed that the sample was collected from

  waterbody                The waterbody the sample was collected from

  location_code            The sampling location code

  huc10                    The 10 digit hydrological unit code for the sampling location

  huc8                     The 8 digit hydrological unit code for the sampling location

  project                  The project that is associated with the sampling

  description              A description of the sampling location

  additional_description   An additional description of the sampling location

  visit_id                 The identification number of the sampling event

  sample_depth             An expanded description of the sampling depth

  analyte                  PFAS analyte

  analyte_value            The analyte concentration in the sample measured in parts per
                           trillion (ppt or ng/L)
  --------------------------------------------------------------------------------------
:::
::::

### Public water supply sampling data

From the [EGLE
website](https://www.michigan.gov/egle/maps-data/mpart-pfas-gis):

*The public water supply results include information from both the State
of Michigan funded drinking water Per- and Polyfluoroalkyl Substances
(PFAS) sampling effort, and ongoing PFAS compliance monitoring of public
water supplies in Michigan. It includes, but is not limited to, sample
location, sample date, and sample results...*

*The combined public water supply results data is representative of the
PFAS sampling locations, with each location having multiple samples
taken, dates for each sample, and the analytical results for each
sample.*

:::: cell
::: cell-output-display
  ---------------------------------------------------------------------------------
  Variable        Description
  --------------- -----------------------------------------------------------------
  geoid           geographic region ID with the first 2 digits being the state
                  Federal Information Processing Standard (FIPS) code and the last
                  3 digits the county FIPS code

  longitude       The longitude coordinate for the sampling location

  latitude        The latitude coordinate for the sampling location

  system_name     Name of water supply system

  system_type     Type of water supply system

  sample_date     The date that the sample was collected

  lab_name_code   Code for processing lab

  analyte         PFAS analyte

  analyte_value   The analyte concentration in the sample measured in parts per
                  trillion (ppt or ng/L)
  ---------------------------------------------------------------------------------
:::
::::

### PFAS sites

This data was last updated on 02/05/2025, and was downloaded on
02/25/2025 from the
[EGLE](https://gis-egle.hub.arcgis.com/maps/17b26cf283624bf49705741e81fde0c4)
website. Cleaned data in a more convenient CSV format is available
[here](https://raw.githubusercontent.com/dilernia/STA418-518/refs/heads/main/Data/pfas_sites.csv):
<https://raw.githubusercontent.com/dilernia/STA418-518/refs/heads/main/Data/pfas_sites.csv>.
From the EGLE website:

*The Michigan PFAS Sites layer is the official list of PFAS sites in
Michigan. This data is updated as new PFAS sites are encountered.*

The original website for the definitions of the site variables is
[here](https://gis-egle.hub.arcgis.com/datasets/egle::michigan-pfas-sites/about):
<https://gis-egle.hub.arcgis.com/datasets/egle::michigan-pfas-sites/about>.

:::: cell
::: cell-output-display
  --------------------------------------------------------------------------------------------------
  Variable                     Type        Description
  ---------------------------- ----------- ---------------------------------------------------------
  geoid                        double      Geographic region ID with the first 2 digits being the
                                           state Federal Information Processing Standard (FIPS) code
                                           and the last 3 digits the county FIPS code

  longitude                    double      Longitude coordinate of sample location

  latitude                     double      Latitude coordinate of sample location

  facility                     character   Name of the site

  county                       character   County where the site is located

  address                      character   Physical address of the project site

  city                         character   City where the project is physically located

  zip_code                     double      Zip code where the project is physically located

  type                         character   Describes the kind of site by type

  residential_wells_sampled    character   Indicates whether residential wells have, or will be
                                           sampled (Domains = Yes, No, TBD, N/A)

  site_lead                    character   Name of contact person

  site_lead_email              character   Contact person email

  site_lead_phone              character   Contact person phone number

  hyperlink                    character   Web address to the site investigation summary

  location                     character   Geographic location description of the site

  military                     character   Indicates if the site is associated with the military

  facility_date                character   Date the site was published on the Michigan PFAS Action
                                           Response Team website

  site_background              character   Background information about the site

  drinking_water_information   character   Information about drinking water quality and safety

  anticipated_activities       character   The state of Michigan's planned or upcoming activities
                                           related to the site
  --------------------------------------------------------------------------------------------------
:::
::::
