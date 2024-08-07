# Terms and Acronyms Common to the Federal LCA Commons
The list of terms and acronyms is alphabetical according to 'Full Name'. Not all terms have an associated abbreviation or acronym. Single quotes are used to denote defined terms when deemed helpful.  

|Acronym or Abbreviation| Full Name| Definition or Descriptive Link
|----|----|----
|Argonne/ANL|Argonne National Laboratory|Visit Argonne's [homepage](https://www.anl.gov/) or their [GREET Tool](https://greet.anl.gov/results)
|APA|American Psychological Association||-|
|-|collaboration server|An openLCA specific server application, maintained by GreenDelta, that allows users to work collaboratively on LCA models, share data, and host public LCA repositories such as those available on [lcacommons.gov](https://www.lcacommons.gov/lca-collaboration/). For more information, see [GreenDelta's Collaboration Server 
|-|context|In the case of the FEDEFL (and often in LCA more broadly), context describes the origin or destination of an elementary flow. Context informs the directionality of an elementary flow. Resource flows are extracted from nature, while emissions are released to nature. [List of FEDEFL contexts](https://github.com/USEPA/Federal-LCA-Commons-Elementary-Flow-List/blob/master/wiki/resources/FEDEFLcontexts.xlsx). For more discussion of context see [EPA's FEDEFL Report](https://cfpub.epa.gov/si/si_public_record_report.cfm?dirEntryId=347251&Lab=NRMRL&simpleSearch=0&showCriteria=2&searchAll=elementary+flows&TIMSType=Published+Report&dateBeginPublishedPresented=07%2F31%2F2019)
|database|project database|In the context of the FLCAC, the term project database is used to refer to a collection of background and foreground LCA processes, flows, product systems. LCIA methods and other data objects as developed by an LCA practitioner(s). A project database is often composed of one or more 'repositories' and novel foreground LCI models that are typically the basis of 'product systems' under study. The goal of the FLCAC is to provide background data and a community of practice to inform consistency in developing project databases. 
|DALY|Disability-Adjusted Life Years|"One DALY represents the loss of the equivalent of one year of full health. DALYs for a disease or health condition are the sum of the years of life lost to due to premature mortality (YLLs) and the years lived with a disability (YLDs) due to prevalent cases of the disease or health condition in a population." from [World Health Organization](https://www.who.int/data/gho/indicator-metadata-registry/imr-details/158#:~:text=Definition%3A-,One%20DALY%20represents%20the%20loss%20of%20the%20equivalent%20of%20one,health%20condition%20in%20a%20population.)
|DOE|Department of Energy|-|
|-|elementary flow|  A material (resource), energy or space that is exchanged with the biosphere. An elementary flow is characterized by a unique combination of 'flowable' and 'context' information and is assigned a 'UUID'.
|endpoint|endpoint indicator|A category of LCIA indicator that expresses characterized impact in terms of damage caused to an area of concern such as the natural environment, human health or resource supply. An example of an endpoint indicator would be the human health impact of particulate matter formation potential expressed in 'Disability-Adjusted Life Years'.
|EPA|Environmental Protection Agency|-|
|EPD|Environmental Product Declaration|A third-party verified report of the environmental impacts of a product. EPDs are developed according to ISO 14025 and the relevant 'product category rule' for that product type. For more information see the [FHWA EPD Tech Brief](https://www.fhwa.dot.gov/pavement/sustainability/hif21025.pdf)
|FEDEFL|Federal Elementary Flow List|Standardized list of elementary flow names, developed by the U.S. Environmental Protection Agency, used in federal LCA work. [FEDEFL GitHub](https://github.com/USEPA/fedelemflowlist)
|FHWA|Federal Highway Administration|[U.S. Federal Highway Administration homepage](https://highways.dot.gov/)
|FLCAC|Federal LCA Commons| [LCA Commons About Us Page](https://www.lcacommons.gov/about-us)
|-|flowable|A general term for the name of a material, energy or space that is exchanged with the biosphere. For more discussion of flowables see [EPA's FEDEFL Report](https://cfpub.epa.gov/si/si_public_record_report.cfm?dirEntryId=347251&Lab=NRMRL&simpleSearch=0&showCriteria=2&searchAll=elementary+flows&TIMSType=Published+Report&dateBeginPublishedPresented=07%2F31%2F2019)
|-|functional unit| The reference unit of a 'product system' within LCA. Results are run and compared on the functional unit. [ISO 14040](https://www.iso.org/standard/37456.html)
|ILCD|International Reference Life Cycle Data|-|
|ISO|International Organization for Standardization|An [independent, non-governmental body](https://www.iso.org/structure.html) with members from national standards boards that develops standard procedures for technical processes, such as life cycle assessment. 
|JSON|JavaScript Object Notation|"A lightweight data-interchange format" from [json.org](https://www.json.org/json-en.html). JSONs are used to house LCA-related data objects within openLCA.
|KML|Keyhole Markup Language|-|
|lib|library| A type of data package limited to read-only access, intended to serve as a dependency of another data package. The library feature in openLCA 2.0 and later versions enables the use of databases together without the need to import them on top of one another. Processes and other elements that are part of a library database are not editable but can be utilized as part of processes or product systems in the main database.
|LCA|Life Cycle Assessment| [United Nations description of environmental LCA](https://www.lifecycleinitiative.org/starting-life-cycle-thinking/life-cycle-approaches/environmental-lca/)
|LCC|Life Cycle Costing|-|
|LCI|Life Cycle Inventory|-|
|LCIA|Life Cycle Impact Assessment|-|
|midpoint|midpoint indicator|"A characterization method that provides indicators for comparison of environmental interventions at a level of cause-effect chain between emissions/resource consumption and the endpoint level." from the European Commission report [Indicators and targets for the reduction of the environmental impact of EU consumption: Overall environmental impact (resource) indicators](https://eplca.jrc.ec.europa.eu/uploads/JRC92824_qms_h08_lcind_deliverable3_final_20141113.pdf). A common example of a midpoint indicator is global climate change potential where impacts are expressed as kg CO<sub>2 </sub>equivalents.
|NAICS|North American Industry Classification System|-|
|NAL|National Agricultural Library|-|
|NETL|National Energy Technology Laboratory|An energy technology laboratory within the U.S. Department of Energy. Visit their [energy data exchange](https://edx.netl.doe.gov/)
|NIST|National Institute of Standards and Technology|A physical science laboratory within the U.S. Department of Commerce. Visit their [science data portal](https://data.nist.gov/sdp/#/)
|NREL|National Renewable Energy Laboratory|An energy technology laboratory within the U.S. Department of Energy. Visit the [NREL Data Catalog](https://data.nrel.gov/)
|oLCA|openLCA|Open source LCA software, data on the FLCAC is provided in formats that are compatible with openLCA. [openLCA Home Pahe](https://www.openlca.org/)
|-|process| A set of related activities that convert inputs into output(s). A network of processes, the 'product system', is used to define the life cycle of a product. Processes are characterized as 'unit processes' or system processes'. For more discussion of processes see [openLCA 2 manual](https://greendelta.github.io/openLCA2-manual/processes/index.html?highlight=process#processes)
|PCR|Product Category Rule|"A set of specific rules, requirements and guidelines for developing Type Ill environmental declarations for one or more product categories." from[ISO 14025](https://www.iso.org/standard/38131.html). See also [EPA's Guidance for Product Category Rule Development](https://cfpub.epa.gov/si/si_public_record_report.cfm?dirEntryId=259406&Lab=NRMRL)
|-||product flow| These are all the flows that are not elementary or waste flows, and represent the materials or energy exchanged between processes within the product system. [openLCA 2 manual](https://greendelta.github.io/openLCA2-manual/flows/index.html)
|repo|repository|A remote or local container in which data are stored under version control, from which a release of contained data can be published. The term repository is often applied to individual data releases (e.g. [USLCI](https://www.lcacommons.gov/lca-collaboration/National_Renewable_Energy_Laboratory/USLCI_Database_Public/datasets)) on the 'collaboration server' or individual GitHub sites (e.g. [FLCAC-Curation](https://github.com/FLCAC-admin/FLCAC-Curation).
|resource|resource flow|A material or energy flow exiting the biosphere, which serves as an LCA process input. 
|SQL|Structured Query Language|-|
|-|system process|"An aggregated life cycle result saved as a process." -from [openLCA 2 manual](https://greendelta.github.io/openLCA2-manual/processes/index.html?highlight=process#processes)
|-|technosphere flow|Intermediate product or service flows that serve as inputs to subsequent processes or comprise the functional unit of a product system. 
|-|unit process|"The  smallest (least aggregated) unit in a production system, for which input and output data are quantified." -from [openLCA 2 manual](https://greendelta.github.io/openLCA2-manual/processes/index.html?highlight=process#processes)
|USDA|U.S. Department of Agriculture|[USDA Ag Data Commons](https://www.nal.usda.gov/services/agdatacommons)
|EPA|U.S. Environmental Protection Agency|[EPA's Open Data resources](https://www.epa.gov/data/enterprise-data-catalog)
|USFS|U.S. Forest Service|An agency within the USDA. Visit the [USFS Research Data Archive](https://www.fs.usda.gov/rds/archive/)
|USLCI|U.S. Life Cycle Inventory database|Database of life cycle inventory data from industry and academia. Visit the [USLCI GitHub Page](https://github.com/FLCAC-admin/uslci-content).
|UUID|Universally Unique Identifiers|Unrepeated alphanumeric code that points to specific database objects, typically within a JSON file. Within openLCA, UUIDs are assigned to processes, flows, product systems, projects, parameters, impact categories and LCIA methods. Link to UUID search in the [openLCA 2 manual](https://greendelta.github.io/openLCA2-manual/introduction/index.html?search=UUID)
|-|waste flow| Waste flows are any substances or objects that the holder needs to dispose of, like by-products with no market value or those requiring more resources to recycle than their economic return. [openLCA 2 manual](https://greendelta.github.io/openLCA2-manual/flows/index.html)









