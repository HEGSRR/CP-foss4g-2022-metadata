## Abstract Expectations

- approach
- results
- concepts
- reasons for consideration
- interest for audience

## Mainstreaming metadata into research workflows to advance reproducibility and open geographic information science

# Abstract

Free and open source software for geospatial analysis (FOSS4G) supports burgeoning possibilities for practicing open and computationally reproducible human-environment and geographical research (Singleton et al 2016).
Open and reproducible research practices may accelerate the pace of scientific discovery and enhance the scientific community's functions of knowledge verification, correction, and diffusion (Rey 2009, Kedron and Holler 2022).
Geospatial metadata provides the foundation for reproducibility and open science and accordingly, requires more support in open source geospatial software.
Following Wilson and others' (2021) five star guide for reproducibility, researchers can achieve four stars by conducting research with open data and software and documenting metadata according to the standards of the International Organization for Standardization (ISO) and OGC (Open Geospatial Consortium).
For Tullis and Kar (2021), metadata is the key to documenting the provenance of research data artifacts, preserving information about every detail of data creation and transformation.
Wilkinson and others' (2016) FAIR Guiding Principles for scientific data management enumerate functions for metadata in each of the principles for research: findable, accessible, interoperable, and reusable.
However, open source geospatial software platforms generally lack the tools necessary for mainstreaming geospatial metadata into the full research workflow in support of more efficient research work and enhanced reproducibility and open science.
This research on metadata is part of a larger human-environment and geographical sciences reproducibility and replicability (github.com/HEGSRR) project aimed at conducting formal reproduction and replication studies in the geographical sciences and integrating reproducibility into undergraduate and graduate level curricula in research methods.

Following the National Academies of Science, Engineering and Medicine (NASEM, 2019), a reproduction study aims find the same results using the same data and methodology as a published study.
A replication study aims to test the findings of a published study by collecting new data and following a similar methodology, which may intentionally modify one or more research parameters.
Together, reproduction and replication studies offer a deep understanding of the original research, test its credibility and generalizability, and enhance the self-corrective mechanisms of the scientific community.
Metadata is information about data, including essential contextual information about the data's spatial structure, attributes, creation, maintenance, access, licensing, and provenance.

A key component of reproducible research is an executable research compendium containing all of the data, code, and narrative required to compile a research publication from raw data (Nust and Pebesma 2021 and the Opening Reproducible Research Project).
Computational notebooks like Jupyter notebooks or R Markdown are commonly used to interweave narrative with code in executable compendia.
In order to maximize replicability and inferential power, the research compendium should begin with a pre-registered research plan prior to data collection, requiring researchers to fully specify metadata for all of the research data and analyzes that they intend to create (Nosek et al. 2018).
It is recommended to store compendia in version tracking systems like Git in order to preserve a full history of changes to the research project.
Finally, the compendium should be published parallel to academic publications so that other researchers can independently re-run, check and verify the analysis, or incorporate the research in future projects.
In order to maximize the findability and legibility of the research compendium for both humans and machines, the overall repository and each of its components must be meticulously documented with metadata according to international standards (Wilkinson et al. 2016, Wilson et al. 2021).

In this three-part research paper, we focus on metadata in research compendia and related research products through all phases of the research workflow.
First, we specify ideal requirements of geospatial metadata in support of reproducible research workflows and open science.
We consider metadata needs at each step of the research process, including proposal writing, pre-analysis registration, ethics review board approval, data collection and analysis, publishing, and reproducing published research.
The metadata software needs assessment is based on literature review of reproducibility and open science, and on teaching and practicing reproducibility with geographic methods.

Second, we review the Dublin Core and International Organization for Standardization (ISO) geospatial metadata standards and popular open source platforms for geospatial research and their support for the requirements of geospatial metadata articulated in the first part.
The scope of the review includes metadata functionality available through spatial analysis software platforms, including R, Python, QGIS, GRASS and SAGA; and it also includes metadata or cataloging tools, including GeoNetwork, GeoNode, the USGS Metadata Wizard, and mdeditor.

Finally, we articulate a vision for open source geospatial metadata software development in support of open and reproducible human-environment and geographical research.
In this vision, metadata software tools shall integrate with executable research compendium to assist researchers with their workflow from inception to publishing and archiving.
The vision builds off our HEGSRR project, in which we independently reproduce and replicate published studies with open source geospatial software, integrate reproduction and replication studies into project-based geographic information science courses, and develop curricula and infrastructure for reproducible research.
Each section of the paper is thus supplemented with experiences and examples drawn from the HEGSRR project.
Of particular relevance, we have already completed seven reproduction or replication studies with graduate and undergraduate students using open source geospatial software, encountering numerous barriers caused by inadequate use or documentation of metadata in research planning, execution, and archiving.
We have also developed a template Git repository compendium for reproducible research and prototyped its use in our studies and teaching, discovering software barriers to documenting metadata and opportunities to integrate metadata into more efficient and reproducible research practices.

We have selected FOSS4G for this research paper in hopes of reaching both the academic audience and developer audience at the conference. We hope to raise awareness in the academic audience of the critical importance of geospatial metadata in each stage of the research workflow. We hope to raise interest in the open source geospatial software community for collaboration on improved support for geospatial metadata in research workflows.
