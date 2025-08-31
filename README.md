# The Loading Lab 🧪

Welcome! This repo is a collection of **lightweight, sandbox-style demos** for common life-science data types.  
Each folder is self-contained and shows how to:

1. **Load** the data into Python
2. Do 1–3 **basic EDA plots or summaries**
3. Point you to **next steps** if you want to dive deeper

The goal: lower the barrier to entry. Once you can *load and peek*, you can explore on your own.


## 📌 Notes
- Note the Disclaimer!
    - The purpose of these demo notebooks are just to get you up to speed and running some fun analyses on common lab data outputs.
    - Don't stop there if (when!) you reach the point of putting this into production.
- Note the Roadmap!
    - I'm completing demos in descending order of the historical level of fun I've had working with the data (...because, why not?) 
    - If there's something particular you'd like me to prioritize, please let me know! Always happy to have an extra data point to help prioritize. 
- Environments
    - I'm making 1 per data type to avoid requirement conflicts.
- Data
    - Links the the README of the respective folders.
    - I'll make an extra "data download" notebook as/when convenient. 

## ⚠️ Disclaimer

The goal of The Loading Lab is to help you get started — fast. These are basic, stand-alone notebooks meant to lower the barrier to entry and make the first steps with real data fun and approachable.

- The notebooks are deliberately written in a quick, exploratory style — not how I’d structure production-quality pipelines in real work.

- Once you’re comfortable loading and plotting data here, the next step is to adopt best practices for serious projects, such as:

    - Using the command line and scripts for reproducibility

    - Writing modular functions and packages instead of monolithic notebooks

    - Adding version control (Git) for your analysis code

    - Managing environments with conda/mamba or pip and pinning versions

    - Building workflows with Snakemake / Nextflow / CWL for maintainability

    - Using Docker/containers when you need portability across systems

    - Writing tests and using continuous integration for long-term reliability

I like the notebook approach here because it makes the repo easy to read and follow along without setup overhead — you can see the logic and outputs inline.

So treat these as “sandbox demos”: once you’re ready to do your own research or production work, start layering on the right habits and tools for scalability and rigor.

Enjoy, and I hope this helps you learn and have fun! 


## ✅ Modules included
- `flow_cytometry/` — FCS files (CyTOF/flow): channels, FSC/SSC, histograms

## 🏗️ Road Map / Under Construction
(Just thinking out loud here....)
- `rnaseq_bulk/` — bulk RNA-seq: counts → QC → toy DE
- `rnaseq_single_cell/` — scRNA-seq: AnnData, PCA/UMAP, quick clustering
- `proteomics_ms/` — proteomics matrices: PCA, heatmap
- `microscopy/` — load microscopy TIFF/PNG, display, histogram, simple segmentation  
- `vcf_variants/` — parse VCF, count SNPs/indels, variant density plots  
- `elisa_plate/` — plate reader CSV → heatmap
- Some QA/QC stuff would be fun --> maybe put it in the specific folder for that data type? Or give QA/QC work it's own folder.
- Automations - same question as the QA/QC.
