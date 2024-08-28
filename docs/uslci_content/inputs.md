# Inputs Field Conventions

[**_Return to TOC_**](../00-sub-handbook-landing.md)

[**Return to Metadata Guidance Tables List**](../02-how-to-publish-in-the-uslci.md#metadata-guidance-tables)

This table includes conventions for the following set of fields in this tab of openLCA:

- [Inputs](#inputs)

### Inputs may include:


- **Resource**: resources from nature, including water, energy, geological flows, land use, and carbon sequestrated from air
- **Ecosystem Services**: provisioning, regulation and maineannce, or cultural services from nature or human modification of ecosystems via technosphere activities; includes land transformation
- **Raw material**: primary or secondary material used to produce a product or reference flow, including intermediary products, semi-finished goods; etc., for example, a refined fuel, chemical, resin, substance, metal alloy, lumber, paper, scrap
- **Energy**: energy inputs from technosphere, e.g., heat, electricity
- **Ancillary**: input Including ancillary materials, transport flows and other services used by an activity but not constituting part of the final product or reference flow; includes materials, transport flows and other services, e.g., lubricant, printing inks, labels, packaging
- **Emission**: emission to nature via air, ground, and water; includes water returned to nature with chemical or physical quality, including temperature, modified from the original source and/or returned to a watershed other than the source
- **Residues**: solid, liquid or gaseous flow, e.g. to a treatment process
- **Co-product**: by-product or co-product of a multi-output process; includes service, transport, etc.
- **Product**: reference product of a system; includes service, transport, etc.
<br>
<br>


<a id="inputs"></a> 
## Inputs

| Field Name | Convention | Examples |
|:---:|:-----|:---------|
|(A) Flow|**Elementary Flows:**<br>Elementary flows should be named based on the **Federal Elementary Flow List (FEDEFL)**. For general elementary flow information, see Highlights 1-14 of the [FEDEFL Nomenclature Guidelines](https://github.com/uslci-admin/uslci-content/blob/dev/docs/submission_handbook/05-FEDEFL%20Guidelines%20-%20Appendix%20Fork.md). See the [EPA FEDEFL Guidance](https://cfpub.epa.gov/si/si_public_record_report.cfm?Lab=NRMRL&dirEntryId=341199) for detailed conventions.<br><br>**Technosphere Flows:**<br>Flow names are based on the USLCI Naming Convention (see [General Information, Name Field Conventions](./general-info.md#general-information). For general product/process flow names, see Rules 12-17 of [Appendix D: ILCD Nomenclature Rules](../04-resources/04-App-D.md). See the full [ILCD Handbook](http://eplca.jrc.ec.europa.eu/uploads/MANPROJ-PR-ILCD-Handbook-Nomenclature-and-other-conventions-first-edition-ISBN-fin-v1.0-E.pdf) for detailed conventions|**Elementary Flow**<br>_'Biological'<br>Hardwood, Resource/Biotic_<br><br>**Technosphere Flow**<br>_EPS virgin resin manufacture; batch suspension polymerization; industry average, at plant_&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|(A) Category|Flow category based on the USLCI Categorization Convention (see [General Information, Name Field Conventions](../field-conventions/general-info.md#general-information))|_Chemical Manufacturing/Resin, Synthetic Rubber, and Artificial Synthetic Fibers and Filaments Manufacturing_|
|(M) Amount|Flow quantity|_0.484_|
|(M) Unit|Flow unit; the openLCA software includes a set of unit groups and units; these units must be used to ensure proper data importation. If these units are not appropriate for one or more of your dataset flows, let your Data Curator know and NREL will assist in adding a unit to the list|_kg_|
|(O) Costs/Revenues|This field is provided for documenting life cycle costing (LCC) data; the currency and costs may be provided for each flow; the costs per unit are automatically generated based on this information and flow amount|_1.45 USD/kg_|
|(O) Uncertainty|Describe flow's data uncertainty. This information is not required, but if provided it increases the process' usefulness. The distribution type, mean, and standard deviation may be provided|_Normal distribution_<br>_Mean = 0.484_<br>_Standard deviation = 0.15_|
|(O) Avoided waste|If there is a scrap or waste flow that is utilized in your process, the flow may be listed as an input to your dataset and marked as an avoided waste|_Bottle waste_|
|(O) Provider|If the flow is produced by more than one process, you may use the drop-down menu to select a default provider|_Aluminum production; hot rolling; production mix, at plant_|
|(O) Data quality entry|Describe the flow's data quality. This information is not required, but if provided it increases the process' usefulness. The flow data quality schema must first be defined on the ‘General information’ tab to be entered for each flow in the ‘Inputs/Outputs’ tab. It is preferred that you use the US EPA data quality schema for process flows. For details on the data quality scheme, see the pull-down menu descriptors in openLCA or the [EPA 2016 Guidance Document on Data Quality Assessment for LCI Data](https://cfpub.epa.gov/si/si_public_file_download.cfm?p_download_id=528687).|_(1;2;1;2;4)_|
|(M) Description|This field is required where applicable. Briefly describe the flow's relationship to the process and assumptions used to obtain the quantitative reference or data quality|_Transport to secondary processing_|

<br><br><br>
[**_Return to TOC_**](../00-sub-handbook-landing.md)
<br><br>
[**Return to Metadata Guidance Tables List**](../02-how-to-publish-in-the-uslci.md#metadata-guidance-tables)
<br><br><br>





  
  
