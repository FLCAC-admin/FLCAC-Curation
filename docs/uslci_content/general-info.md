# General Information Field Conventions

[**_Return to TOC_**](../00-sub-handbook-landing.md)

[**Return to Metadata Guidance Tables List**](../02-how-to-publish-in-the-uslci.md#metadata-guidance-tables)

This set of tables includes the following conventions for this tab in openLCA:
- [General Information](#general-information)
- [Quantitative Reference](#quantitative-reference)
- [Time](#time)
- [Geography](#geography)
- [Technology](#technology)
- [Data Quality](#data-quality)<br>

<a id="general-information"></a> 
## General Information

| Field Name | Convention | Examples |
|:---:|:-----|:---------|
   | (M) Description | A legible overview of the process description, i.e., technical scope, functional unit, system boundaries, and any other information needed for unambiguous data interpretation and application.<br><br>**FUNCTIONAL UNIT**: Measure of the function of the studied system quantified to provides a reference to which the inputs and outputs can be related. <br><br>**TECHNICAL SCOPE**: Cradle-to-gate, cradle-to-grave, gate-to-gate, gate-to-grave. <br><br>**SYSTEM BOUNDARIES**: included processes, i.e., boundaries between the technosphere and nature; geographic and temporal scope; boundaries between this and other technosphere systems. Examples of included processes are: raw material acquisition; manufacturing/processing/refining; distribution/transport; production and use of fuels, electricity, and heat; use and maintenance of products; disposal of process waste and products; recovery of used products via reuse, recycling, and energy recovery; ancillary materials manufacturing; manufacture, installation, maintenance, and decommissioning of capital equipment; additional operations, such as lighting, heating, service personnel. |<br>_This gate-to-gate unit process is for net production of one kilowatt-hour of electricity supply from a coal-fired plant with co-generation of steam in Four Corners Area, United States. The studied system includes all processes, from washed coal delivery through to power generation, including treatment of cooling water, of a combined heat and power plant with conventional steam cycle within a circulating fluidized bed.The fuel is 100% washed bituminous coal extracted from Rocky Mountain regional mines located within 500 km of the plant. Data are from one coal-powered base load plant so no aggregation was performed but is representative of typical coal-based power facility in that region._<br><br>_Technical data assumed for the studied plant:_<br><br>_Annual time of operation (hours): 4 000_<br><br>_Normal annual electricity production (GW⋅h): 40_<br><br>_Annual steam production (TJ): 30_<br><br>_Assumed lifetime (years): 40_<br><br>_Electricity production, net during 40 years (TW⋅h): 1,6_<br><br><br> |
   |(M) Category|The category/subcategories schema follows North American Industry Classification System (NAICS). Categorize process by placing it in the proper folder in the process tree (using the USLCI categorization convention as a guide); Once the JSON-LD USLCI Database zip file has been uploaded, the categories display and can guide the placement of your datasets in the USLCI categorization scheme; use the format main category (2-digit NAICS category/4-digit NAICS subcategory) schema (see [Appendix E: 2017 NAICS United States Structure](../04-resources/04-App-E.md)).|_22: Utilities/2211: Electric Power Generation, Transmission and Distribution_ <br><br> _31-33: Manufacturing/3253: Pesticide, Fertilizer, and Other Agricultural Chemical Manufacturing_|
  |(A) Version|Per the ILCD, the data set version; the first two digits indicate major updates, while the second two digits refer to minor revisions and error corrections; the final three digits are used for automatic and internal version counting during dataset development; Unless discussed in advance with the Data Curator, the value will be generated automatically by openLCA|_01.00.000_|
  |(A) UUID|<a id="uuid"></a> 32-digit Universally Unique Identifier (UUID) for the data set<sup>[**[2]**](#fn2)</sup>|_961fad56-bde2-4fbe-8895-5be03461729b_|
  |(A) Last change|The date and time when the dataset was last saved|_2018-04-01T17:38:55-0600_|
  |(M) Infrastructure process|Checking this box indicates that the process includes infrastructure requirements in its inventory. Leave this box unchecked if infrastructure requirements are not included in the process|_False_|
  <br>
    
  <a id="quantitative-reference"></a> 
  ## Quantitative Reference
  
  | Field Name | Convention | Examples |
|:---:|:-----|:---------|
|(M) Quantitative reference|When you create a new process, this is the basis by which all the process flows are scaled; often the functional unit; the quantitative reference must be one of the process output flows; the output flows appear in a pull-down menu by default (See Rule 16: “Quantitative flow properties” name field, in [Appendix D: ILCD Nomenclature Rules](../04-resources/04-App-D.md).|_Scanner; Kodak Alaris i940 desktop scanner; Global supply chain; 1 unit, 1.55 kg_&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
 <br>
 
<a id="time"></a> 
## Time

| Field Name | Convention | Examples |
|:---:|:-----|:---------|
|(M) Start date|Start date for the time period that the process represents. The date format is MM/DD/YYYY|_01/01/2017_|
|(M) End date|End date for the time period that the process represents. The date format is MM/DD/YYYY|_12/31/2017_|
|(M) Description|Additional information regarding the temporal characteristics and period that the process represents. Examples can include explanation of the valid time period, any temporal aggregation, data collection period, seasonal/annual variations, and carbon provenance. <br><br> NOTE: The valid time span is often identical to the time of the data collection, i.e., unless projections or other forecasts have been applied. Limitations on the validity in valid time span can include future technology shifts, planned measurement improvements, or specific seasons. |_This unit process is representative of operations from 2014-2015. Water consumption varied seasonally but was averaged over an annual period._|
 <br>
 
<a id="geography"></a> 
## Geography

| Field Name | Convention | Examples |
|:---:|:-----|:---------|
|(M) Location|The geographic area to which the unit process data were collected or refer. NREL recommends that the geography reference the highest geographic resolution possible. Indicate ‘US’ unless higher geographic resolution is available. Use [ISO 3166-2](https://www.iso.org/iso-3166-country-codes.html) code indicating the process’ geographic location if it is a US state. If the data are not a US state, also describe the locations in the geography ‘Description’ field|_US-CO_|
|(O) KML|Keyhole Markup Language (KML) file which allows users to create a coordinate point, bounding box or polygon indicating the geographic area the process represents; external KML files cannot be submitted|_Polygon [-77.92, 39.55… -77.92, 39.55]_|
|(M) Description|Description of the process' geographic representativeness and any geographic aggregation methods as well as name(s) and production volume(s) or capacity of specific included site(s), where applicable. Any geographical information on where the process, inputs and/or outputs occur is useful for end-users in considering region-specific aspects such as average insolation, temperature, wind speeds, and precipitation levels, etc. that affect e.g., landfill decomposition, fate and transport of emissions, etc.|_This process is representative of production in the state of Colorado. Production data were aggregated across five sites ranging from eastern to western Colorado._&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
 <br>
 
<a id="technology"></a> 
## Technology
| Field Name | Convention | Examples |
|:---:|:-----|:---------|
|(M) Description|A short (i.e., 1-3 paragraphs), general description of the process intended technical scope, representativeness, and relevance, i.e., applicability of the process. Include the following information (if applicable):&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br><ul><li>Process design including sub-processes, unit operations, and/or other activities (anthropogenic or natural) included in the process.</li><li>Material selection and quality.</li><li>Operational conditions and representativeness; i.e., quantitative or qualitative assessment of the degree to which the data reflect the true population of interest.</li><li>A description of any fate and transport modeling.</li><ul>|_This process represents the production of "Calcium carbonate, ground, 20 microns, at plant" using average technologies for the United States from 2015-2016.<br><br>The process includes three sub-processes: Quarry Operations; Transport and Plant Processing. Quarry Operations includes the following unit operations: mechanical extraction; primary crushing; screening; and intermediate storage of calcium carbonate rock (marble, limestone, or chalk). Transport includes the transport of materials from Quarry Operations to Plant Processing via barge, train, or truck. Plant processing which includes jaw crushing, washing, impact crushing, ball milling to particle size, and then classifying. Material selection and quality represent industry averages from the contiguous United States. Operational conditions represent industry averages from the contiguous United States.Fate and transport modeling was not considered for this process._|
 <br>
  
<a id="data-quality"></a> 
## Data Quality
  
| Field Name | Convention | Examples |
|:---:|:-----|:---------|
|(M) Process schema|Currently, the only default process schema for data quality available in openLCA is adapted from ecoinvent; other data quality schemes may be downloaded from openLCA and imported. It is preferred that you use the US EPA data quality system for the process schema|_US EPA data quality system_|
|(M) Data quality entry|Selecting the “not specified” link opens the Pedigree matrix, in which you can select the cardinal indicators for flow reliability, temporal correlation, geographical correlation, further technological correlation, and data collection methods (i.e., completeness). For details on the data quality scheme, see the pull-down menu descriptors in openLCA or the [EPA 2016 Guidance Document on Data Quality Assessment for LCI Data](https://cfpub.epa.gov/si/si_public_file_download.cfm?p_download_id=528687).|_(1;2;1;1;1)_|
|(O) Flow schema|Currently, the only default flow schema for data quality available in openLCA is adapted from ecoinvent; it is preferred that you use the US EPA data quality system for the flow schema.|_US EPA data quality system_|
|(O) Social schema|Currently, the only default social schema for data quality available in openLCA is adapted from ecoinvent|_ecoinvent data quality system_&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|

<br><br><br>


  
  <a id="fn1"></a>
>[[1]](#general-information). Note, when creating a new process in openLCA, it is possible to create a waste treatment process selecting a waste flow previously created as quantitative reference (the reference input of this process).

<a id="fn2"></a>
>[[2]](#uuid). Data exported from SimaPRO in the ecospold file format do not have a UUID. Therefore, if a SimaPRO-generated ecospold file is imported into openLCA, the software will assign a new UUID and can cause breaks in the linking between existing flows and processes in the USLCI Database.

<br><br><br>

[**_Return to TOC_**](../00-sub-handbook-landing.md)
<br><br>
[**Return to Metadata Guidance Tables List**](../02-how-to-publish-in-the-uslci.md#metadata-guidance-tables)
<br><br><br>





  
  
  
  


