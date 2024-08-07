# Frequently Asked Questions

## Using and Accessing Data

### Federal LCA Commons (FLCAC)
<details>
 <summary><b>What is the Federal LCA Commons?</b></summary>
 
Official definition of the Federal LCA Commons (FLCAC) can be found on the [About Us](https://www.lcacommons.gov/about-us) page of the lcacommons.gov website.

The FLCAC is a collaborative project across several agencies of the U.S. federal government intended to make life cycle inventory (LCI) data available across agencies and to the general public.
The FLCAC also looks to establish community resources and best practices for using and conducting life cycle assessments (LCA). 

- List of LCI and LCIA [repositories available on the FLCAC](https://www.lcacommons.gov/lca-collaboration/)
- Homepage for [FLCAC resources](https://github.com/FLCAC-admin/FLCAC-Curation)

</details>

<details>
 <summary><b>What is the FLCAC collaboration server?</b></summary>

The FLCAC collaboration server is a server application that allows repository owners to work together on openLCA databases and publish databases to the Federal LCA Commons. Local openLCA databases can be connected to the collaboration server and information can be transferred. More information on openLCA collaboration servers can be found [here](https://www.openlca.org/collaboration-server/).
</details>

<details>
 <summary><b>What is the difference between USLCI and the FLCAC?</b></summary>

The Federal LCA Commons (FLCAC) is a collaborative project across several agencies of the U.S. federal government intended to make life cycle inventory (LCI) data available across agencies and to the general public. The FLCAC hosts multiple LCI repositories one of which is the U.S. Life Cycle Inventory database (USLCI). USLCI is an LCI portal for datasets submitted by consulting, academia, & industry associations, the database includes several hundred process LCIs ranging from fuels combustion, transport, metals, chemicals, plastics, and glass to paper. More information on USLCI can be found [here](https://github.com/FLCAC-admin/uslci-content) and USLCI specific FAQS are available [here](https://github.com/FLCAC-admin/uslci-content/blob/dev/docs/submission_handbook/03-frequently-asked-questions.md).
 
</details>

### Finding Data
<details>
 <summary><b>How do I see what data exists on the FLCAC?</b></summary>

Data on the FLCAC can be accessed via the [FLCAC website](https://lcacommons.gov), select "Browse repositories" on the landing page, select the repository of interest, and browse the elements included in that repository by opening folders. 

You can also search for processes across all repositories via the search function in the top right, filters are available to refine your search to specific repositories and elements of repositories. Data on the FLCAC can also be explored within openLCA by downloading the data from the FLCAC and importing them into an openLCA database. You can look through the elements in the navigation pane or the search function.
</details>

<details>
 <summary><b>How do I find impact assessment methods?</b></summary>

Impact assessment methods aligned with the Federal Elementary Flow List (FEDEFL) and Federal LCA Commons data are available in two forms:
- [LCIA Methods without flows](https://www.lcacommons.gov/lcia-methods-without-flows):
These JSON-LD files do not contain the flow objects, only the characterization factors.
They can be downloaded and imported into any openLCA database.
The "No flows" versions of methods must be imported _into_ a database that contains flows, otherwise the methods will not appear in the database.
Updating a local database with new data which contains new elementary flows (e.g., importing a new process from a repository on the FLCAC) may result in new, uncharacterized flows in the database.
In these cases, the "No flows" methods should be **re-imported** to enusre that all elementary flows are charcterized.

- LCIA Methods repositories: [Repositories](https://www.lcacommons.gov/lca-collaboration/) are available for TRACI2.1 and ReCiPe which contain the methods and all relevant flow objects.
These repositories are useful for reviewing all characterization factors for flows in the FEDEFL.
They can be downloaded and imported into a user's local database.
However doing so will also import _all_ FEDEFL flows characterized by the method, often resulting in over 100,000 flow objects.

See [Life Cycle Impact Assessment Methods](LCIAmethods.md) for additional details.

</details>

<details>

 <summary><b>What LCIA methods are currently harmonized for use with LCI data on the FLCAC?</b></summary>

The LCIA methods listed in the following table are currently available on the FLCAC and have been harmonized to align with the federal elementary flow list using the [LCIAFormatter](https://github.com/USEPA/LCIAformatter).

|LCIA Data|Provider|Link|
|---|---|---|
|TRACI 2.1|US Environmental Protection Agency|[Tool for Reduction and Assessment of Chemicals and Other Environmental Impacts](https://www.epa.gov/chemical-research/tool-reduction-and-assessment-chemicals-and-other-environmental-impacts-traci)|
|ReCiPe 2016 Midpoint|National Institute for Public Health and the Environment (The Netherlands)|[LCIA: the ReCiPe Model](https://www.rivm.nl/en/life-cycle-assessment-lca/recipe)|
|ReCiPe 2016 Endpoint|National Institute for Public Health and the Environment (The Netherlands)|[LCIA: the ReCiPe Model](https://www.rivm.nl/en/life-cycle-assessment-lca/recipe)|
|ImpactWorld+ Midpoint*|International Reference Center for Life Cycle of Products, Services and Systems (CIRAIG)|[ImpactWorld+](http://www.impactworldplus.org/en/team.php)|
|ImpactWorld+ Endpoint*|International Reference Center for Life Cycle of Products, Services and Systems (CIRAIG)|[ImpactWorld+](http://www.impactworldplus.org/en/team.php)|
|IPCC GWP|Intergovernmental Panel on Climate Change (IPCC)| |
|FEDEFL Inventory Methods|US Environmental Protection Agency|[FEDEFL Inventory Methods](https://github.com/USEPA/LCIAformatter/wiki/Inventory-Methods)|

TRACI version 2.2 with updated Eutrophication Factors is currently being harmonized for compatibility with FLCAC data. 

Additional LCIA methods such as CML, Ecopoint, eco-indicator, EDIP2003, EPS, IMAGE 3, LIME, LUCAS, MEEup, ILCD and NAMEA are not currently available in a harmonized format. Flow mapping would be required to use these impact assessment methods with FLCAC data.

See [Life Cycle Impact Assessment Methods](LCIAmethods.md) for additional details.

</details>

### openLCA

<details>
 <summary><b>How do I use data from the FLCAC in openLCA?</b></summary>

Download whole repositories or repository elements (e.g., processes and flows) on the FLCAC as a JSON-LD file type (if prompted, select which version of openLCA you are working in, newer versions of openLCA are 2.0 and later). Do not unzip this file.

Then, open openLCA, create a new empty database, right click on the database, select 'import', select 'file', and navigate to the downloaded JSON-LD file in your file explorer. [YouTube video on this topic](https://www.youtube.com/watch?v=YLao5jC5b_0&list=PLmIn8Hncs7bFUOyXZNGXwG4LtdoTfLz6Q&index=3)
</details>

<details>
 <summary><b>How do I calculate LCIA results (e.g., climate change, eutrophication potential, etc.) for data on the FLCAC?</b></summary>

To calculate LCIA assessment results, your repository needs two elements: a database made up of process LCIs and an LCIA assessment method. See the questions above for information on which impact assessment methods are available. Importing impact assessment methods is done the same way as importing repositories (right click on database, select 'import', select 'file', navigate to the relevant file). If using the no-flows methods then import the methods file after importing the process database. You can verify that LCIA methods were imported by opening the 'Indicators and parameters' and checking the 'Impact assessment methods' folder.

Once your database has both processes and a method, open up the process that you would like to calculate results for, on the 'General information' tab select 'Create product system'. For most processes the default product system selections are okay. More information on these options can be found in the openLCA manual [here](https://greendelta.github.io/openLCA2-manual/prod_sys/Creating.html). Select 'Finish' and evaluate the 'Reference' section and the 'Model Graph' in your product system. Then, select 'Calculate', set the 'Allocation method' as 'As defined in process', choose your impact assessment method (if there are no options here then the LCIA methods were not imported), and use the default settings for the remaining fields. Select 'Finish' and navigate through the results tabs to view results.

There are many variations of this process to run results so please reference the [openLCA manual](https://greendelta.github.io/openLCA2-manual/how-to-use.html) for more information, the steps above provide instructions for running a basic process.

</details>

<details>
 <summary><b>Why are the impact assessment methods that I imported into openLCA not showing up in my database?</b></summary>

Two problems could be occurring:
1. Your methods did not import. To solve this issue please follow the instructions above under 'How do I calculate LCIA results for data on the FLCAC?'. If this does not solve the problem then ensure that problem 2 is not occurring and then contact the data curators at FederalLCACommons@erg.com.
2. You are using the "No flows" version of a method and imported the method package before a process database with flows. The "No flows" versions of methods must be imported _into_ a database that contains flows, otherwise the methods will not appear in the database.
</details>

<details>
 <summary><b>What is a library?</b></summary>

The library feature in openLCA 2.0 and later versions enables the use of databases together without needing to import them on top of one another. A library serves as a read only database that can easily be combined with other databases. Processes and other elements that are part of a library database are not editable but can be utilized as part of processes or product systems in the main database. 

Libraries are beneficial for the current set-up of the FLCAC as they allow for multiple distributed repositories to be self-contained, while still promoting interoperability between repositories. The connections provided by libraries benefit multiple repositories on the FLCAC. It’s important to note that libraries are currently an experimental feature in openLCA and will be updated based on user feedback and identified issues.

</details>

<details>
 <summary><b>What is a provider?</b></summary>

A provider in openLCA is the upstream process that produces a flow. Providers can be chosen in the 'Inputs/Outputs' tab in openLCA under the 'Provider' column for product and waste flows. Product and waste flows can have one or more provider, but elementary and cut-off flows do not have a provider because these flows have no upstream process producing them. It is important that data providers select the provider fields in their inventories to ensure that a flow is connected to the correct upstream process.
</details>

## Data Submission
<details>
 <summary><b>How do I submit data to the Federal LCA Commons (FLCAC)?</b></summary>

Submission processes vary for each repository, so it is recommended to reach out to the repository managers/owners to submit data or inquire about the specific data submission process.
The USLCI submission process is currently recommended as the default FLCAC submission process. The submission handbook may be found [here](https://github.com/FLCAC-admin/uslci-content/blob/dev/docs/submission_handbook/00-sub-handbook-landing.md) and a YouTube training video that covers this process is located [here](https://www.youtube.com/watch?v=jecyDLHu6OQ).
The current FLCAC-Curation repository also includes various resources for preparing your data for the FLCAC. 

Here is a brief overview of the data preparation process: 
- Map elementary flows to FEDEFL
- Map technosphere flows to those that exist in the FLCAC repositories, or create new processes that produce the desired flows. Cut-off flows can also be created if needed, but these are not recommended.
- Import the data into openLCA, this can be done before or after the mapping process.
- Align the processes and flows with the NAICS folder structure.
- Complete the metadata for each process as described in the [USLCI metadata guidance tables](https://github.com/FLCAC-admin/uslci-content/blob/dev/docs/submission_handbook/02-how-to-publish-in-the-uslci.md#metadata-guidance-tables).
- Export the processes intended for submission and submit them to the repository owner/manager.
  - If you are the repository owner/manager then you will integrate the new processes into the existing database and push it to the collaboration server.

</details>

<details>
 <summary><b>How do I align my elementary flows with the Federal Elementary Flow List?</b></summary>

All data on the Federal LCA Commons must use elementary flows that conform to the [Federal Elementary Flow List](https://cfpub.epa.gov/si/si_public_record_report.cfm?Lab=NRMRL&dirEntryId=347251).
For instructions on mapping your flows, see [here](https://github.com/USEPA/fedelemflowlist/wiki/Getting-Started-with-FEDEFL#mapping-a-dataset)
</details>

<details>
 <summary><b>How do I align my technosphere flows the FLCAC?</b></summary>

Technosphere flows (i.e., product or waste flows) that come from another database (e.g., ecoinvent, Agri-footprint, GaBi, etc.) must be mapped to technosphere flows that exist within the FLCAC repositories or new processes should be created that produce these flows. Cut-off flows may be created if neither of the previous options are possible. 

To map technosphere flows, you may either create a new process within openLCA and manually add the desired technosphere flows to your life cycle inventory (LCI) or you may use [openLCA's flow mapping function](https://www.openlca.org/flow-mapping-feature/) which allows you to apply mappings to your whole database.

</details>

<details>
 <summary><b>How do I align my dataset with the NAICS folder structure?</b></summary>

All data on the Federal LCA Commons must use the North American Industry Classification System (NAICS) folder structure [NAICS - Census Bureau](https://www.census.gov/naics/).
To align new or existing processes and flows with NAICS, import the [Commons Core database](https://www.lcacommons.gov/lca-collaboration/Federal_LCA_Commons/Fed_Commons_core_database/datasets) to add the NAICS folder structure to your openLCA database and then organize flows and processes into the relevant folders. Use the NAICS Census Bureau link above to determine the appropriate 4 digit NAICS code. 
</details>

<details>
 <summary><b>I have specific questions about data submission to the FLCAC, who do I reach out to?</b></summary>

Please submit questions to the FLCAC data curators via the [Issues page](https://github.com/FLCAC-admin/FLCAC-Curation/issues) or email us at FederalLCACommons@erg.com.
</details>

## Other Questions

### Data Review and Data Quality
<details>
 <summary><b>What review process does data on the FLCAC undergo?</b></summary>

Data posted to the FLCAC is subjected to the review process as described in process-level metadata. The FLCAC Data Curators do not perform an additional critical review of submitted data or check for ISO compliance. 

Currently, metadata fields are not consistently filled out within USLCI or all federal LCA or LCIA repositories on the FLCAC. Data users will need to assess the available metadata to ensure that utilized LCI datasets meet the data quality standards associated with their project scope. 

The FLCAC Data Curator is engaged in an ongoing task to assess data quality on the FLCAC and retroactively assign data quality scores that will help practitioners assess the sufficiency of a given dataset for their project.

Moving forward the FLCAC Data Curator will also work to ensure that metadata is consistently filled out for all new data submissions. At this time, there is no plan to retroactively update process metadata (aside from data quality scores) for data previously submitted to the FLCAC.

</details>

### Other LCA Software

<details>
 <summary><b>How do I use data from the FLCAC in other software?</b></summary>

Multiple LCA platforms outside of openLCA support repositories that are provided on the FLCAC, although not all of this data is up to date. For this reason, when using FLCAC data on other platforms please check the version or release date and compare to what is currently hosted on the [FLCAC](https://www.lcacommons.gov/lca-collaboration/). Please contact the individual software companies for more information on the repositories supported.
</details>

### LCA Terminology

<details>
 <summary><b>What is a cut-off flow?</b></summary>

A cut-off flow is a flow that is a placeholder or a dummy flow. These flows are used when no relevant flows in a database exists. It is not recommended to use these flows in your life cycle inventory if possible. In openLCA results, cut-off flows will appear in your inventory results, but will not contribute to impact category results.
</details>





