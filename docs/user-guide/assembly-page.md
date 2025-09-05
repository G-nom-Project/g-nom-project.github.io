## Intro section
The first section of the assembly page is made up of a grey band detailing scientific name and the custom name of the assembly. A silouette of the species can be supplied via SVG at source e.g. from [Phylopic](https://www.phylopic.org/).
![Assembly Head](../assets/screenshots/AssemblyPage.png){ align=center }
The first section below the band details taxon specific information. These include an image, scientifc and common names as well a short header text and longer info text. The complete NCBI lineage is displayed in a separate field.

The remainder of the page is made up of four collapsible sections, which will be discussed in detail below:

1. Assembly Information
2. Annotation completeness
3. Taxonomic classification
4. Genome Browser

## Assembly Information
![Assembly Collapsible](../assets/screenshots/AssemblyPageCollapsible1.png){ align=center }
The assembly information sections contains G-nom internal information as well common quality metrics and statistics. This includes sequence and contig size statistics as well as N50 and GC content. To assess the completeness of the assembly / related annotation, please check out the BUSCO and fCAT results in the next section.

## Annotation completeness
![Assembly BUSCO](../assets/screenshots/AssemblyPageBUSCO.png){ align=center }
The annotation completeness section presents visualizations for BUSCO and fCAT results. The plot differentiates between Complete (Single-copy), Complete (Duplicated), fragmented and missing. Please refer to the documentation of the underlying tools ([BUSCO](https://busco.ezlab.org/busco_userguide.html#interpreting-the-results) | [fCat](https://f1000research.com/posters/11-1091)) for guidance on how to interpret the results.

## Taxonomic assignment :material-account-hard-hat-outline:
!!! warning taXaminer-dashboard

    The taXaminer-dashboard project is currently being re-structured to be published as a singular react component. This feature should be considered unstable until the migration is complete.    
    

The taxonomic assignment section includes the complete [dashboard](https://github.com/BIONF/taxaminer-dashboard) for the visualization of taXaminer results. Additionally, it integrates with you G-nom account and the genome browser.


## Genome Browser
![Assembly Browser](../assets/screenshots/AssemblyPageBrowser.png){ align=center }
The genome browser section embeds a smaller version of the [JBrowse](https://jbrowse.org/jb2/) genome browser. Per default, all available tracks will be loaded. It links to selected genes in the taXaminer dashboard, allowing you to explore the genomic neighbourhood. For detailed investigation of browser tracks, consider using the [Full-screen browser](/user-guide/browser/).