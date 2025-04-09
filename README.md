**User Guide:**

# Creating a Data-to-Knowledge Package
  
**Note:** This document is a draft. Please send your questions, comments, and suggestions to m.konkol[at]52north.org.
This user guide provides instructions on how to create a Data-to-Knowledge Package (DKP) as described in this paper (<INSERT LINK>).

**Problem statement:**
1.	Reusing open reproducible research is challenging.
2.	Research materials are often published in different repositories and not connected.
	
**Solution:**
1.	Based on a reproducible basis (code + data + computational environment), further applications including virtual labs, web API services, and workflows are built to encourage reuse.
2.	The Data-to-Knowledge Package links these materials and applications to create a connection between them.
   
**Target audience:**
Users who have an analysis pipeline and would like to create a DKP out of it.

# What is a Data-to-Knowledge Package?
  
The Data-to-Knowledge Package (DKP) is a framework designed to enhance the reusability of computational research outputs by integrating key digital research assets. It addresses challenges in reproducibility by linking essential components, including data, code, virtual labs, web API services, and computational workflows. Unlike traditional research compendiums, the DKP does not duplicate data but instead provides structured links to existing resources, reducing redundancy and ensuring synchronization.
At its core, the DKP comprises a reproducible basis—data and a structured code toolbox—enabling the derivation of additional research components. By offering self-contained, reusable functions, it facilitates adaptation in various research contexts. The DKP also supports computational environments, mitigating technical barriers for users with diverse expertise levels.
A primary goal of the DKP is to promote the reuse of research by allowing researchers to inspect, execute, and modify analysis workflows efficiently. This approach streamlines the research cycle, fosters collaboration, and accelerates knowledge generation. Moreover, its metadata structure ensures findability and accessibility, aligning with the FAIR Principles. Ultimately, it provides a scalable solution for improving transparency, credibility, and the impact of reproducible research. Before you start creating your own DKP, feel free to visit a demo DKP to get an impression on the AquaINFRA Interaction Platform and on Zenodo.

# How can I create a DKP?
**Technologies**
In this user guide, we use the following technologies to create a DKP:

●	[R]([url](https://www.google.com/search?client=firefox-b-d&q=r+tutorial)) and python to write the source code
●	GitHub to host the toolbox
○	Note: GitLab is possible, too, but at some point you will need to create a Pull Request to the Galaxy platform, which is only possible via GitHub.
●	Docker to containerize the source code
●	MyBinder to provide the virtual lab
●	OGC API Processes to provide OGC API Web Services based on pygeoapi
●	Galaxy to develop and run workflows
●	ro-crate to create the DKP
●	Zenodo to store the materials
You will need access to a server to deploy the OGC API Process using, for instance, pygeoapi. If you are a member of the AquaINFRA project and would like to deploy your processes on the AquaINFRA server, please get in touch with us (<mail_address>).



