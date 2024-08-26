# Flow Mapping

Flow mapping is the process of relating {term}`elementary  flow`s in one dataset to similar flows in another dataset. In the context of the FLCAC, typically users are mapping the elementary flows in a third-party dataset (such as Ecoinvent or a dataset from the openLCA Neuxs) to the {term}`Federal Elementary Flow List` (FEDEFL).

:::{note} Technosphere flows
Flow mapping can also be performed on {term}`technosphere flow`s, for example when identifying an alternate source of background LCI data.
:::

Flow mapping is a critical step for accurate and complete LCIA flow characterization when using multiple LCI repositories in a single project database. In order for LCIA methods available on the FLCAC to fully capture the elementary flows present in a project database or product system they must be mapped to the FEDEFL as this flow list is the basis of LCIA methods on the commons.

:::{seealso}

- [Guidance for Mapping a Dataset](https://github.com/USEPA/fedelemflowlist/wiki/Getting-Started-with-FEDEFL#mapping-a-dataset)
- [Mapping within openLCA](https://github.com/USEPA/fedelemflowlist/wiki/FEDEFL-in-openLCA#mapping-a-dataset-within-openlca)
:::