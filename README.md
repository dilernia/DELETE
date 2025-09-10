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
<div id="xjxkzdfeuo" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#xjxkzdfeuo table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#xjxkzdfeuo thead, #xjxkzdfeuo tbody, #xjxkzdfeuo tfoot, #xjxkzdfeuo tr, #xjxkzdfeuo td, #xjxkzdfeuo th {
  border-style: none;
}

#xjxkzdfeuo p {
  margin: 0;
  padding: 0;
}

#xjxkzdfeuo .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#xjxkzdfeuo .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#xjxkzdfeuo .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#xjxkzdfeuo .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#xjxkzdfeuo .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#xjxkzdfeuo .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#xjxkzdfeuo .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#xjxkzdfeuo .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#xjxkzdfeuo .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#xjxkzdfeuo .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#xjxkzdfeuo .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#xjxkzdfeuo .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#xjxkzdfeuo .gt_spanner_row {
  border-bottom-style: hidden;
}

#xjxkzdfeuo .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#xjxkzdfeuo .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#xjxkzdfeuo .gt_from_md > :first-child {
  margin-top: 0;
}

#xjxkzdfeuo .gt_from_md > :last-child {
  margin-bottom: 0;
}

#xjxkzdfeuo .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#xjxkzdfeuo .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#xjxkzdfeuo .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#xjxkzdfeuo .gt_row_group_first td {
  border-top-width: 2px;
}

#xjxkzdfeuo .gt_row_group_first th {
  border-top-width: 2px;
}

#xjxkzdfeuo .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#xjxkzdfeuo .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#xjxkzdfeuo .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#xjxkzdfeuo .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#xjxkzdfeuo .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#xjxkzdfeuo .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#xjxkzdfeuo .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#xjxkzdfeuo .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#xjxkzdfeuo .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#xjxkzdfeuo .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#xjxkzdfeuo .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#xjxkzdfeuo .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#xjxkzdfeuo .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#xjxkzdfeuo .gt_left {
  text-align: left;
}

#xjxkzdfeuo .gt_center {
  text-align: center;
}

#xjxkzdfeuo .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#xjxkzdfeuo .gt_font_normal {
  font-weight: normal;
}

#xjxkzdfeuo .gt_font_bold {
  font-weight: bold;
}

#xjxkzdfeuo .gt_font_italic {
  font-style: italic;
}

#xjxkzdfeuo .gt_super {
  font-size: 65%;
}

#xjxkzdfeuo .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#xjxkzdfeuo .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#xjxkzdfeuo .gt_indent_1 {
  text-indent: 5px;
}

#xjxkzdfeuo .gt_indent_2 {
  text-indent: 10px;
}

#xjxkzdfeuo .gt_indent_3 {
  text-indent: 15px;
}

#xjxkzdfeuo .gt_indent_4 {
  text-indent: 20px;
}

#xjxkzdfeuo .gt_indent_5 {
  text-indent: 25px;
}

#xjxkzdfeuo .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#xjxkzdfeuo div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>

  Variable                 Description
  ------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------
  geoid                    geographic region ID with the first 2 digits being the state Federal Information Processing Standard (FIPS) code and the last 3 digits the county FIPS code
  longitude                The longitude coordinate for the sampling location
  latitude                 The latitude coordinate for the sampling location
  lab_sample_id            The sample ID provided by the analytical laboratory
  site_code                The sampling location name
  coc_sample_id            The sample ID listed on chain of custody provided to the analytical laboratory
  sample_type              An expanded description of what type of sample was collected
  lab_name                 The name of the analytical laboratory used for analysis of the sample
  lab_job_name             The analytical laboratories job/work order name
  collection_date          The date that the sample was collected
  analysis_method          The analysis method used by the analytical laboratory to analyze the sample
  dilution_factor          The dilution factor used by the analytical laboratory during sample preparation
  analysis_date            The date that the analysis was conducted by the analytical laboratory
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
  analyte_value            The analyte concentration in the sample measured in parts per trillion (ppt or ng/L)

</div>
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
<div id="rombjdticb" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#rombjdticb table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#rombjdticb thead, #rombjdticb tbody, #rombjdticb tfoot, #rombjdticb tr, #rombjdticb td, #rombjdticb th {
  border-style: none;
}

#rombjdticb p {
  margin: 0;
  padding: 0;
}

#rombjdticb .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#rombjdticb .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#rombjdticb .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#rombjdticb .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#rombjdticb .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#rombjdticb .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#rombjdticb .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#rombjdticb .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#rombjdticb .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#rombjdticb .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#rombjdticb .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#rombjdticb .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#rombjdticb .gt_spanner_row {
  border-bottom-style: hidden;
}

#rombjdticb .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#rombjdticb .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#rombjdticb .gt_from_md > :first-child {
  margin-top: 0;
}

#rombjdticb .gt_from_md > :last-child {
  margin-bottom: 0;
}

#rombjdticb .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#rombjdticb .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#rombjdticb .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#rombjdticb .gt_row_group_first td {
  border-top-width: 2px;
}

#rombjdticb .gt_row_group_first th {
  border-top-width: 2px;
}

#rombjdticb .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#rombjdticb .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#rombjdticb .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#rombjdticb .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#rombjdticb .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#rombjdticb .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#rombjdticb .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#rombjdticb .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#rombjdticb .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#rombjdticb .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#rombjdticb .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#rombjdticb .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#rombjdticb .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#rombjdticb .gt_left {
  text-align: left;
}

#rombjdticb .gt_center {
  text-align: center;
}

#rombjdticb .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#rombjdticb .gt_font_normal {
  font-weight: normal;
}

#rombjdticb .gt_font_bold {
  font-weight: bold;
}

#rombjdticb .gt_font_italic {
  font-style: italic;
}

#rombjdticb .gt_super {
  font-size: 65%;
}

#rombjdticb .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#rombjdticb .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#rombjdticb .gt_indent_1 {
  text-indent: 5px;
}

#rombjdticb .gt_indent_2 {
  text-indent: 10px;
}

#rombjdticb .gt_indent_3 {
  text-indent: 15px;
}

#rombjdticb .gt_indent_4 {
  text-indent: 20px;
}

#rombjdticb .gt_indent_5 {
  text-indent: 25px;
}

#rombjdticb .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#rombjdticb div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>

  Variable        Description
  --------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------
  geoid           geographic region ID with the first 2 digits being the state Federal Information Processing Standard (FIPS) code and the last 3 digits the county FIPS code
  longitude       The longitude coordinate for the sampling location
  latitude        The latitude coordinate for the sampling location
  system_name     Name of water supply system
  system_type     Type of water supply system
  sample_date     The date that the sample was collected
  lab_name_code   Code for processing lab
  analyte         PFAS analyte
  analyte_value   The analyte concentration in the sample measured in parts per trillion (ppt or ng/L)

</div>
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
<div id="nelertzpff" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#nelertzpff table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nelertzpff thead, #nelertzpff tbody, #nelertzpff tfoot, #nelertzpff tr, #nelertzpff td, #nelertzpff th {
  border-style: none;
}

#nelertzpff p {
  margin: 0;
  padding: 0;
}

#nelertzpff .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#nelertzpff .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#nelertzpff .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#nelertzpff .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#nelertzpff .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#nelertzpff .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#nelertzpff .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#nelertzpff .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#nelertzpff .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#nelertzpff .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#nelertzpff .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#nelertzpff .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#nelertzpff .gt_spanner_row {
  border-bottom-style: hidden;
}

#nelertzpff .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#nelertzpff .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#nelertzpff .gt_from_md > :first-child {
  margin-top: 0;
}

#nelertzpff .gt_from_md > :last-child {
  margin-bottom: 0;
}

#nelertzpff .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#nelertzpff .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#nelertzpff .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#nelertzpff .gt_row_group_first td {
  border-top-width: 2px;
}

#nelertzpff .gt_row_group_first th {
  border-top-width: 2px;
}

#nelertzpff .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#nelertzpff .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#nelertzpff .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#nelertzpff .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#nelertzpff .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#nelertzpff .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#nelertzpff .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#nelertzpff .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#nelertzpff .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#nelertzpff .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#nelertzpff .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#nelertzpff .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#nelertzpff .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#nelertzpff .gt_left {
  text-align: left;
}

#nelertzpff .gt_center {
  text-align: center;
}

#nelertzpff .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#nelertzpff .gt_font_normal {
  font-weight: normal;
}

#nelertzpff .gt_font_bold {
  font-weight: bold;
}

#nelertzpff .gt_font_italic {
  font-style: italic;
}

#nelertzpff .gt_super {
  font-size: 65%;
}

#nelertzpff .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#nelertzpff .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#nelertzpff .gt_indent_1 {
  text-indent: 5px;
}

#nelertzpff .gt_indent_2 {
  text-indent: 10px;
}

#nelertzpff .gt_indent_3 {
  text-indent: 15px;
}

#nelertzpff .gt_indent_4 {
  text-indent: 20px;
}

#nelertzpff .gt_indent_5 {
  text-indent: 25px;
}

#nelertzpff .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#nelertzpff div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>

  Variable                     Type        Description
  ---------------------------- ----------- -------------------------------------------------------------------------------------------------------------------------------------------------------------
  geoid                        double      Geographic region ID with the first 2 digits being the state Federal Information Processing Standard (FIPS) code and the last 3 digits the county FIPS code
  longitude                    double      Longitude coordinate of sample location
  latitude                     double      Latitude coordinate of sample location
  facility                     character   Name of the site
  county                       character   County where the site is located
  address                      character   Physical address of the project site
  city                         character   City where the project is physically located
  zip_code                     double      Zip code where the project is physically located
  type                         character   Describes the kind of site by type
  residential_wells_sampled    character   Indicates whether residential wells have, or will be sampled (Domains = Yes, No, TBD, N/A)
  site_lead                    character   Name of contact person
  site_lead_email              character   Contact person email
  site_lead_phone              character   Contact person phone number
  hyperlink                    character   Web address to the site investigation summary
  location                     character   Geographic location description of the site
  military                     character   Indicates if the site is associated with the military
  facility_date                character   Date the site was published on the Michigan PFAS Action Response Team website
  site_background              character   Background information about the site
  drinking_water_information   character   Information about drinking water quality and safety
  anticipated_activities       character   The state of Michigan\'s planned or upcoming activities related to the site

</div>
:::
::::
