# Exploring Retrieval Augmented Generation (RAG) for Drug Repusposing using LLMs

**Authors:** Fuad Al Abir and Akhil Goparaju

Department of Computer Science, College of Arts and Sciences, University of Alabama at Birmingham, AL 35205, USA


## Dataset Description
We have used the Drug Repurposing Knowledge Graph (DRKG) dataset (https://github.com/gnn4dr/DRKG) for the project. DRKG is a comprehensive biological knowledge graph relating genes, compounds, diseases, biological processes, side effects and symptoms. DRKG includes information from six existing databases including DrugBank, Hetionet, GNBR, String, IntAct and DGIdb. It includes 97,238 entities belonging to 13 entity-types; and 5,874,261 triplets belonging to 107 edge-types. These 107 edge-types show a type of interaction between one of the 17 entity-type pairs (multiple types of interactions are possible between the same entity-pair), as depicted in the figure below.

![DRKG relationship diagram](https://raw.githubusercontent.com/gnn4dr/DRKG/master/connectivity.png)

## Project Objective

To build synergized **[KG-LLM model](https://arxiv.org/pdf/2306.08302.pdf)** that can advance the state-of-the-art drug discovery, our project aimed to build a prototype with **Retrieval Augmented Generation** on **Knowledge Graphs,** harnessing the power of **open-source LLMs**.

## Project Structure
files: data/ notebook/ imgs/

requirement:

compatibility: cheaha

## Exploratory Data Analysis

## Dataset Preparation

https://drive.google.com/drive/folders/1p1md-1wlaTtKmRDJKJHUsHCjsK_u-XJV?usp=sharing

## Retrieval Augmented Generation on Knowledge Graph

## Fine-tuning LLM

## Discussion

- At first, we aimed to implement RAG on Graph a.k.a. Graph RAG. Thus, we have explored graph databases like [neo4j](https://neo4j.com/), [nebula-graph](https://www.nebula-graph.io/), [aws neptune](https://aws.amazon.com/neptune/) and some others that can support Graph RAG. However, the free tier of the technologies are not feasible for our dataset as we have ~0.4M nodes and ~5.8M edges. This feasibility study took apporimately 20 hours of work.
## Contributions

- **Background Research and Problem Formulation:** Fuad Al Abir
- **Dataset Preparation:** Fuad Al Abir
- **Exploration of RAG:** Fuad Al Abir
- **Exploring Graph RAG solutions:** Akhil Goparaju, Fuad Al Abir
- **Finetuning LLM:** Akhil Goparaju
- **Readme.md:** Fuad Al Abir, Akhil Goparaju
## Acknowledgements

 - To Dr. Osborne, for encouraging us to pick up a "difficult" problem for the project.
 - To the authors of DRKG from Ning Lab, OSU for this comprehensive graph dataset.
 - We have extensively used [llama-index library](https://docs.llamaindex.ai/en/stable/) for RAG experiments and learned from their youtube tutorials.
 - ❤️ for 🤗 and the open-source LLM community.