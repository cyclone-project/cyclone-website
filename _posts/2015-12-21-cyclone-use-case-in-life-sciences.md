---
title: CYCLONE use cases in Life Sciences
---
#### CYCLONE use cases in Life Sciences
Bioinformatics deals with the collection and efficient analysis of biological data, particularly genomic information from DNA sequencers. The capability of modern sequencers to produce terabytes of information coupled with low pricing (less than US$1000 for a human genome), and causes a "data deluge" that is being experienced by researchers in this field.

<!-- more -->

To analyze these data, the scientific and industrial community daily use bioinformatics software that is characterized by a high degree of fragmentation: literally hundreds of different software packages are regularly used for scientific analyses with an incompatible variety of dependencies and a broad range of resource requirements. For this reason, the bioinformatics community has strongly embraced cloud computing with its ability to provide customized execution environments and dynamic resource allocation. 
The French Institute of Bioinformatics - IFB ([www.france-bioinformatique.fr](http://www.france-bioinformatique.fr)) consists of a national hub, the IFB-core, and 34 bioinformatics platforms (PF) grouped into 6 regional centers spanning the entire French territory. The IFB currently deployed two cloud facilities on its own premises, one in IFB-core (Orsay, France) and another one in the platform IFB-GenOuest (Rennes, France), and two others in collaborations with the local computing centers in Lille and Strasbourg. In the next years, the IFB aims to deploy a federated cloud infrastructure over the regional PFs. This cloud infrastructure is devoted to the French life science community, research and industry, with services for the management and analysis of life science data.

#### Leveraging technical areas of the CYCLONE project

The CYCLONE consortium has identified several concrete bioinformatics use cases that aim to address some specific well-identified limitations. For example, regarding the key technical areas of the CYCLONE project, Cloud Access Management through cloud proxies and Matchmaking, Brokering, and Mediation of Cloud Resources will provide the IFB with features to access other cloud infrastructures than the current national IFB’s, to integrate the future cloud infrastructures that will be deployed by the regional IFB’s platform, and also to access external cloud infrastructures from academic or commercial providers. Naturally, the infrastructure users, for example biomedical staff analyzing human biomedical data or researchers analyzing genome sequences, will benefit from these features while accessing the system and carrying out their analyses. Two bioinformatics use cases are already deployed on the CYCLONE infrastructure. 

#### Use case "Securing human biomedical data"

The first deployed bioinformatics use case “Securing human biomedical data“ is a single-VM application requiring enhanced security features such as a trusted federated authentication mode and a deployment done only on certified (by the French Health Ministry) cloud infrastructure. The cloud appliance NGS-Unicancer is developed by the bioinformatics platform of the Centre Léon Bérard (Lyon, France, [www.synergielyoncancer.fr](www.synergielyoncancer.fr)) in the context of the project NGS-Clinique (INCA - Institut National du Cancer). It provides a simple web interface to launch the biomedical genomic analysis pipeline. The appliance was enhanced by the Federation Provider developed by TUB and is ready for on-demand deployment on the IFB-core’s cloud infrastructure. The user deploys the appliance NGS-Unicancer through the IFB’s web interface in “1-click” and uses the CYCLONE federation provider to get access to the VM web interface based on its identity in the federation. The user can then easily upload its data, run the analysis and get the results.

#### Use case "Cloud virtual pipeline for microbial genomes analysis"

The second bioinformatics use case “Cloud virtual pipeline for microbial genomes analysis“ is developed by the platform IFB-MIGALE (Jouy-en-Josas, France, [migale.jouy.inra.fr](http://migale.jouy.inra.fr)). This application requires several components: a user web interface, a relational postgreSQL database, and a complete computing cluster with a master and several nodes to perform the data-intensive analyses. This infrastructure already running in a classical static way on bare-metal servers in IFB-MIGALE premises was ported to the cloud and extended with a « 1-click » deployment features by using SlipStream recipes. The image was exported from the IFB’s cloud and registered in the StratusLab Marketplace. Afterwards, IFB-core wrote a deployment recipe based on SlipStream that instantiates the complete application with all the required VMs on the CYCLONE infrastructure.


*Read more in the deliverable [D3.1](http://www.cyclone-project.eu/assets/images/deliverables/Evaluation%20of%20Use%20Cases.pdf).*
