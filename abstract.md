# Open geographic information science depends upon metadata

Free and open source software for geospatial analysis supports burgeoning possibilities for practicing open and computationally reproducible human-environment and geographical research (Singleton et al 2016), for example in cyberGIS communities for open geospatial science.
Open and reproducible research practices may accelerate the pace of scientific discovery and enhance the scientific community's functions of knowledge verification, correction, and diffusion (Rey 2009, Kedron and Holler 2022).
Metadata provides the foundation for open and reproducible research and scientific data management, but there is an urgent need to develop user-friendly open source metadata management tools for research with open source geospatial software.
In this three-part paper, I first review literature on open and reproducible science to substantiate the key functions and requirements of geospatial metadata from proposal development and pre-analysis registration through publishing, archiving, and reproducing published research.
I then review existing metadata standards and popular open source platforms for geospatial research and their support for the requirements of geospatial metadata articulated in the literature review.
Finally, I articulate a vision for open source geospatial metadata software development in support of open and reproducible human-environment and geographical research.
This vision is based on the literature and software reviews, lessons learned from formally reproducing published studies in the geographic sciences with open source software, and teaching open reproducible geographic information science to undergraduate and graduate geography students.
This research is relevant to FOSS4G contributors interested in enhancing the utility and uptake of open source geospatial software in the research community, to geospatial scientists working on enhancing the reproducibility of their own work, and to geospatial research funding agencies and data archives interested in developing open and reproducible science practices.

## Open and reproducible science

Following Wilson et al's (2021) five star guide for reproducibility, researchers can achieve four-star status by conducting research with open data and software and documenting metadata according to the standards of the International Organization for Standardization (ISO) and OGC (Open Geospatial Consortium).
For Tullis and Kar (2021), metadata is the key to documenting the provenance of research data artifacts, preserving information about every detail of data creation and transformation.
Wilkinson et al's (2016) FAIR Guiding Principles for scientific data management enumerate functions for metadata in each of the principles for research: findable, accessible, interoperable, and reusable.
Each principle is supported by metadata encoded with machine- and human-readable standards.

### Research Design

Metadata should facilitate three major requirements of open and reproducible research design: ethical review, data management plans, and study preregistration.

Most research projects involving human subjects must register a research protocol with an Institutional Review Board (IRB) or Research Ethics Committee for assessment of ethical treatment and protection of the interests of research subjects.
Ethical reviews require specification of sampling procedures, data to be collected, and protocols for storage, access, and protection of confidentiality.  

Major funding sources, including the National Institutes of Health (NIH), National Science Foundation (NSF), and European Research Council (ERC) require data management plans for research grants.
Grants financed with public money increasingly view research data as a public good required to be published in an accessible digital archive and to be findable through searchable metadata.

The predictive power of scientific research relies on researchers' ability to confirm theoretically-deduced hypotheses by testing novel data-- implying that researchers need rely on metadata to specify and preregister research protocols prior to accessing raw data.
Researchers should be able to understand the structure and characteristics of secondary data sources from metadata without accessing the raw data itself.
The ability to do so is important for reducing the need to "explore" the data prior to specifying a research protocol, unintentionally leading to problems of bias, p-hacking and  multiple hypothesis testing.
Metadata for secondary sources should be sufficient to allow researchers to specify research pre-analysis plans without previewing the raw data, thereby enhancing replicability and inferential power by reducing bias in the specification and testing of hypotheses.

### Research Practice

As geospatial scientists conduct research, metadata provides three essential functions.

First, metadata can reduce uncertainty and problems of construct validity, especially when researchers use secondary data.
Metadata should provide context on the production of data used in research, including data dictionaries, ontologies, and information about (spatial) sampling, precision, error, and post-collection processing.

it can provide a record of data provenance by specifying each step of data transformation in the research process (Tullis and Kar 2021). Second, metadata can reduce uncertainty within research teams and between data providers and researchers by providing data dictionaries for attributes with ontological clarification.

The open research community is increasingly calling for the use of research compendia for computational research.
These are structured repositories for research projects containing the computational environments, data, and codified research procedures required to reproduce the study's findings.
The repositories are commonly maintained in a version control system, e.g. Git, in order to maintain a history of every change to the research project over time.
Open geographic information science would benefit from a standardized structure to research compendia, organizing data into raw, scratch/temporary, and derived directories and further into publicly shareable and private or embargoed directories.
This data organization should be structured, indexed, and documented with metadata within repositories to facilitate accessibility and reuse.
The repository as a whole should have a project-level readme document and metadata to facilitate findability and meta-analyses. 

### Research Publishing and Archiving

## Metadata Standards

The ISO standards for geospatial metadata contain information about metadata authorship, data authorship, spatial and temporal extent, coordinate systems, data format, spatial resolution, data dictionaries for attributes, licenses, and access protocols.

- Dublin Core standards for project-level metadata
- OGC standard for geographic information (extent, CRS)
- Human and machine readability-- XML & KML or JSON & GEOJSON

## FOSS4G Software

The FOSS4G software ecosystem includes desktop GIS (e.g. QGIS, GRASS, SAGA, gvSIG), web and catalog services (e.g. GeoNetwork and GeoNode)

The XXX component of geospatial metadata should clearly explain accessibility protocols.
Researchers are often constrained from sharing their data due to proprietary licenses or confidentiality.
In such cases, data may be treated for with techniques such as simulation, sampling, or randomization.
This data requires  
Thoroughly documented metadata must stand in for data that cannot be shared by researchers due to constraints of proprietary or confidential licenses, conveying enough information about inaccessible data for other researchers to design replication studies testing the original findings with new data.

## Vision

Geospatial metadata software should support all steps of the research process from initial research design through to publishing and archiving.
At the research design phase, software should support researchers by integrating metadata into their research proposal data management plans, institutional review board research protocols,
human subjects protocols.
This implies both ability to import metadata for secondary data sources and other published research projects, as well as to author metadata for proposed creation of raw and derived data.
- crawl and update / audit research compendia
- integrate with software for writing data management plans,
