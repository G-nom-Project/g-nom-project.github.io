

All data imported into G-nom is stored in a hierarchy originating the the NCBI Taxonomy. Each genome assembly is linked to a species with a unique NCBI Taxonomy ID. G-nom uses an internal copy of the NCBI ``taxdump`` as a reference which is updated automatically every two weeks (system administrators can adjust this service interval).
``` mermaid

flowchart TD
    Genus --> A@{ shape: processes, label: "Species" }
    A@{ shape: processes, label: "Species" } --> B@{ shape: processes, label: "Assemblies" }
    B@{ shape: processes, label: "Assemblies" } --> Genome
    B@{ shape: processes, label: "Assemblies" } --> C@{ shape: processes, label: "Mappings" }
    B@{ shape: processes, label: "Assemblies" } --> D@{ shape: processes, label: "Annotations" }
    B@{ shape: processes, label: "Assemblies" } --> E@{ shape: processes, label: "Analyses" }
```
Additional data referencing or analysing the genome assembly can be [imported](./import.md). This includes genomic annotations and mappings as well as BUSCO, fCAT and taXaminer analyses. All entities presented in the diagram have additional metadata associated with them which is handled by G-nom automatically. In some cases e.g. species, additional hand-curated data such as Descriptions, Images or Geodata can be added using the [taxon editor](./taxon-editor.md) and will be displayed on the [assembly page](./assembly-page.md).

!!! warning Taxon Editor

    Currently, the taxon Editor only supports editing species-level taxa.

All data at or below assembly level is access-controlled, allowing users to decide who can read / edit their imported data.